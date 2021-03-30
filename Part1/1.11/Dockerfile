FROM openjdk:12

COPY /spring-example-project .

RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]