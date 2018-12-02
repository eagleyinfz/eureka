
FROM ${env.DOCKER_REGISTRY_ADDR}/openjdk:8u181-jdk
VOLUME /tmp
COPY target/lib/*.jar /app/lib/
RUN rm -f /app/lib/servlet-api-2.5.jar
CMD ["/usr/bin/java", "-Djava.security.egd=file:/dev/./urandom", "-cp", "/app/lib/*", "${start-class}"]

