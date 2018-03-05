FROM java:latest

#RUN yum -y update 

#RUN yum -y install java-1.8.0-openjdk-devel

#RUN yum -y install wget

RUN wget http://ftp.yz.yamagata-u.ac.jp/pub/network/apache/tomcat/tomcat-7/v7.0.85/bin/apache-tomcat-7.0.85.tar.gz 
RUN tar xzvf /apache-tomcat-7.0.85.tar.gz

COPY ./*.war /apache-tomcat-7.0.85/webapps/

CMD /apache-tomcat-7.0.85/bin/catalina.sh run
