FROM maven:3.3-jdk-8 as builder
COPY . /build/
WORKDIR /build/p323line/helloworld-ws/
RUN mvn clean install

FROM java:8-jre
RUN wget http://ftp.byfly.by/pub/apache.org/tomcat/tomcat-8/v8.5.32/bin/apache-tomcat-8.5.32.tar.gz
RUN tar -xzvf apache-tomcat-8.5.32.tar.gz -C /opt/
COPY --from=builder /build/p323line/helloworld-ws/target/helloworld-ws.war /opt/apache-tomcat-8.5.32/webapps/
RUN chmod +x /opt/apache-tomcat-8.5.32/bin/catalina.sh
EXPOSE 8080
CMD ["/opt/apache-tomcat-8.5.32/bin/catalina.sh", "run"]
