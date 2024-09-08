# ----------------------------------
# Pterodactyl Core Dockerfile
# Environment: Java
# Minimum Panel Version: 0.6.0
# ----------------------------------
FROM container-registry.oracle.com/graalvm/jdk:17

MAINTAINER GraphicHealer, https://github.com/GraphicHealer/Pterodactyl-GraalVM-Yolk/issues

RUN microdnf -y --best install curl ca-certificates openssl git tar bash sqlite fontconfig \
    && microdnf clean all \
    && useradd -d /home/container -m container

USER container
ENV  USER=container HOME=/home/container

WORKDIR /home/container

COPY ./../entrypoint.sh /entrypoint.sh

CMD ["/bin/bash", "/entrypoint.sh"]
