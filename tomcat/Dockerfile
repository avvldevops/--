FROM ubuntu:18.04
ENV CATALINA_HOME /usr/share/tomcat9
ENV PATH $CATALINA_HOME/bin:$PATH
RUN mkdir -p "$CATALINA_HOME"
ENV CATALINA_BASE /var/lib/tomcat9
RUN apt update && \
apt install default-jdk -y && \
apt install tomcat9 -y
EXPOSE 8080
WORKDIR $CATALINA_HOME
CMD ["catalina.sh", "run"]
