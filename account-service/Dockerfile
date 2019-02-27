FROM java:8-jre
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/account-service.jar /app/
CMD ["java", "-Xdebug", "-Xrunjdwp:server=y,transport=dt_socket,address=7892,suspend=n", "-Xmx200m", "-jar", "/app/account-service.jar"]

EXPOSE 6000 7892