FROM adoptopenjdk/openjdk14:alpine-jre
COPY target/*.jar app.jar
ENV JAVA_OPTS=""
EXPOSE 9002
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]