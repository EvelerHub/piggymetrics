FROM java:8-jre
MAINTAINER Alexander Lukyanchikov <sqshq@sqshq.com>

ADD ./target/config.jar /app/
CMD ["java", "-Xdebug", "-Xrunjdwp:server=y,transport=dt_socket,address=7891,suspend=n", "-Xmx200m", "-jar", "/app/config.jar"]

HEALTHCHECK --interval=30s --timeout=30s CMD curl -f http://config:8888/actuator/health || exit 1

EXPOSE 8888 7891