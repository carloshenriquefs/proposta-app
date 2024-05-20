FROM openjdk:17

COPY target/proposta-app-1.0.jar app.jar

COPY wait-for-it.sh wait-for-it.sh

RUN chmod +x wait-for-it.sh

EXPOSE 8080

ENTRYPOINT ["./wait-for-it.sh", "rabbit-mq:5672", "--", "java", "-Duser.language=pt", "-Duser.country=BR", "-jar", "app.jar"]