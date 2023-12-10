FROM openjdk:22-ea-27-jdk-slim
WORKDIR /app
COPY target .
CMD ["java", "-jar", "spring-boot-data-jpa-0.0.1-SNAPSHOT.jar", "--spring.config.location=classes/application.properties"]
