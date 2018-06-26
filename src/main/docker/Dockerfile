FROM base/java8:1.0
ADD docker_spring_boot.jar /opt/app.jar
RUN sh -c 'touch /opt/app.jar'
ENV JAVA_OPTS=""
ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /opt/app.jar" ]
