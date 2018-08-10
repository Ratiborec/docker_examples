FROM alpine:3.2 
LABEL maintainer="Mikhail Znak"
RUN   apk update && apk add nginx

EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]

