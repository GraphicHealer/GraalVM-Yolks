# ----------------------------------
# Pterodactyl Core Dockerfile
# Environment: Java
# Minimum Panel Version: 0.6.0
# ----------------------------------
FROM container-registry.oracle.com/graalvm/jdk-ee:latest

MAINTAINER GraphicHealer, https://github.com/GraphicHealer/Pterodactyl-GraalVM-Yolk/issues

RUN yum install -y curl ca-certificates openssl git tar bash sqlite fontconfig \
    && yum clean all \
    && rm -rf /var/cache/yum \
    && useradd -D --home-dir /home/container -m container

USER container
ENV  USER=container HOME=/home/container

WORKDIR /home/container

COPY ./../entrypoint.sh /entrypoint.sh

CMD ["/bin/bash", "/entrypoint.sh"]
