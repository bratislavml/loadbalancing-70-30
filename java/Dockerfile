#FROM 412335208158.dkr.ecr.us-east-1.amazonaws.com/sprout-java8:latest
FROM openjdk:11

# drop the jar+config in the container
RUN mkdir /srv/java-webserver
COPY java-webserver.jar /srv/java-webserver

WORKDIR /srv/java-webserver
#CMD /usr/bin/java -jar /srv/java-docker-example/java-docker-example.jar server /srv/java-docker-example/config.yml
#CMD /usr/bin/java -jar /srv/java-docker-example/java-webserver.jar server
ENTRYPOINT ["java","-jar", "java-webserver.jar"]