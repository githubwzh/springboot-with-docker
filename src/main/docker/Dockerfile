FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD springboot-with-docker-0.0.1-SNAPSHOT.jar  app.jar
#http://www.simapple.com/363.html
#COPY . /hehe
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]