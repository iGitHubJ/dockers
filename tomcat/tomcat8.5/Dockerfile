FROM shangdc/jdk8

MAINTAINER sdc "898596025@qq.com"  

RUN mkdir -p /data/reformer/project/logs

RUN apt-get update

ADD apache-tomcat-8.5.23.tar.gz /data/reformer/project

WORKDIR /data/reformer/project

RUN mv apache-tomcat-8.5.23 tomcat

ENV CATALINA_HOME /data/reformer/project/tomcat

VOLUME /data/reformer/project/logs
VOLUME ${CATALINA_HOME}/logs

EXPOSE 8080

CMD ["/data/reformer/project/tomcat/bin/catalina.sh", "run"]