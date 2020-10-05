Jenkins server: http://18.215.116.181:8080/
Artifatcory server:
App server: 


Continuous Integration
=====================








Continuous Delivery
======================









Continuous Deployment
==========================





Pull Request Buiulders
==========================



Develop 
===============


Master cut
===================




Dokcker image
=====================
$vi Dockerfile
FROM tomcat:8.0-alpine

LABEL maintainer="krishnamaram2@gmail.com"

ADD ./Student.war /usr/local/tomcat/webapps/

EXPOSE 8080

CMD ["catalina.sh", "run"]

$docker image build -t myimage .

$docker container  run -d -name mycontainer  -p 8080:8080 myimage


AMI using Packer
==================
