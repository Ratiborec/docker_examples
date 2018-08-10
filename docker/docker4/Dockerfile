FROM java:8-jre
RUN wget http://ftp.byfly.by/pub/apache.org/tomcat/tomcat-8/v8.5.32/bin/apache-tomcat-8.5.32.tar.gz
RUN tar -xzvf apache-tomcat-8.5.32.tar.gz -C /opt/
RUN chmod +x /opt/apache-tomcat-8.5.32/bin/catalina.sh
EXPOSE 8080
CMD ["/opt/apache-tomcat-8.5.32/bin/catalina.sh", "run"]


