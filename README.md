# webapp

Continuous Integration








Continuous Delivery









Continuous Deployment






Pull Request Buiulders



Develop 



Master cut




Dokcker image
=====================
FROM tomcat:8.0-alpine

LABEL maintainer="krishnamaram2@gmail.com"

ADD ./Student.war /usr/local/tomcat/webapps/

EXPOSE 8080

CMD ["catalina.sh", "run"]


AMI using Packer
==================
