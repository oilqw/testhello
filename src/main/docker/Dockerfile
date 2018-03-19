#FROM frolvlad/alpine-oraclejdk8:slim
#VOLUME /tmp
#ADD demo-service-ver-0.0.1.jar app.jar
#RUN sh -c 'touch /app.jar'
#ENV JAVA_OPTS=""
#ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]
FROM stand_jkd18:v1.0
ENV JAVA_HOME /app/jdk18
ENV CLASSPATH $JAVA_HOME/jre/lib/rt.jar:$JAVA_HOME/lib/dt.jar:$JAVA_HOME/lib/tools.jar
ENV PATH $PATH:$JAVA_HOME/bin
RUN /bin/bash -c 'source /etc/profile;echo $JAVA_HOME'
EXPOSE 8080