FROM openjdk:17-jdk-slim

ARG JAR_FILE=./build/libs/*.jar

COPY ${JAR_FILE} /app.jar

EXPOSE 8080

ENTRYPOINT ["java", "-Dspring.profiles.active=prod", "-Duser.timezone=Asia/Seoul", "-jar", "/app.jar"]
