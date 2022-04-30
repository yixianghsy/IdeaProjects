#FROM openjdk:8u181-jdk-alpine
#VOLUME /tmp
#ADD e3-content-service-0.0.1-SNAPSHOT.jar app.jar
#RUN bash -c 'touch /app.jar'
#EXPOSE 8082
#ENTRYPOINT ["java","-XX:+UnlockExperimentalVMOptions"," -XX:+UseCGroupMemoryLimitForHeap","-jar","/app.jar"]

FROM openjdk:8u181-jdk-alpine
VOLUME /tmp
ADD e3-content-service-0.0.1-SNAPSHOT.jar app.jar
RUN bash -c 'touch /app.jar'
EXPOSE 8021
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]