FROM                           maven:3.9.9-amazoncorretto-21-debian as build
RUN                            useradd roboshop
RUN                            mkdir /app
RUN                            chown -R roboshop:roboshop /app
WORKDIR                        /app
RUN                            code/* /app/
RUN                            mvn clean package
RUN                            mv target/shipping-1.0.jar /app/shipping.jar



FROM                            openjdk:25-slim-bullseye
RUN                             mkdir /app
WORKDIR                         /app
COPY                            --from=build /app/shipping.jar /app/shipping.jar

