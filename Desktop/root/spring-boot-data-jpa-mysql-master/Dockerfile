FROM openjdk:22-ea-27-jdk-slim
WORKDIR /app
COPY target/spring-boot-data-jpa-0.0.1-SNAPSHOT.jar .
EXPOSE 8080
CMD ["java", "-jar", "spring-boot-data-jpa-0.0.1-SNAPSHOT.jar", "--spring.config.location=classes/application.properties"]
