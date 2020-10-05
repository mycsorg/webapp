Jenkins server: http://18.215.116.181:8080/

Artifatcory server: http://52.21.14.220:8081

App server: 


Continuous Integration
=====================








Continuous Delivery
======================









Continuous Deployment
==========================





Pull Request Buiulders
==========================
https://medium.com/@mreigen/integrate-jenkins-builds-into-github-pull-requests-33bc053d6210



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
