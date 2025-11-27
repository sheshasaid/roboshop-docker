FROM maven:3.9 AS build
WORKDIR /app
COPY pom.xml .
COPY src ./src
RUN mvn clean package

FROM openjdk:17
WORKDIR /app
COPY --from=build /app/target/shipping-1.0.jar shipping.jar
CMD ["java", "-jar", "shipping.jar"]
