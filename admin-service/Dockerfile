FROM java:8-jre
MAINTAINER Alex Eveler <alexander.eveler@gmail.com>

ADD ./target/admin-service.jar /app/
CMD ["java", "-Xdebug", "-Xrunjdwp:server=y,transport=dt_socket,address=7890,suspend=n", "-Xmx200m", "-jar", "/app/admin-service.jar"]

EXPOSE 9999 7890