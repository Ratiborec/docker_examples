FROM centos
LABEL maintainer="Mikhail Znak"
RUN yum install -y httpd web-assets-httpd && \
    yum clean all
RUN echo "my httpd container" > /var/www/html/index.html
EXPOSE 80
ENTRYPOINT ["httpd"]
CMD ["-DFOREGROUND"]
