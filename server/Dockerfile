FROM gradle:8.10.0-jdk22 AS build

WORKDIR /app

COPY . /app

RUN chmod +x ./gradlew

RUN ./gradlew assemble

CMD ["java -jar target/tracker-server.jar" ]