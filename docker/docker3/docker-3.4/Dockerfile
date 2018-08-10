FROM centos
LABEL maintainer="Mikhail Znak"
RUN 	yum install epel-release -y && \
	yum install -y nginx && \
	yum clean all
COPY ./nginx /etc/nginx/nginx.conf
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
