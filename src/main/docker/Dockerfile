FROM 10.1.9.199:5000/centos/javaweb:base
VOLUME /tmp
ADD docker_spring_boot.jar app.jar
RUN sh -c 'touch /app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]