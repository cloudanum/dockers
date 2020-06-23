ARG BASE_CONTAINER=cloudanum/base_minimal_scipy_pyspark
FROM $BASE_CONTAINER

LABEL maintainer="Cloudanum"

USER root

ENV Z_VERSION="0.8.2"
ENV LOG_TAG="[ZEPPELIN_${Z_VERSION}]:" \
    Z_HOME="/zeppelin" \
    LANG=en_US.UTF-8 \
    LC_ALL=en_US.UTF-8
RUN mkdir /zeppelin
RUN echo "$LOG_TAG Download Zeppelin binary"
RUN wget -O /tmp/zeppelin-${Z_VERSION}-bin-all.tgz http://archive.apache.org/dist/zeppelin/zeppelin-${Z_VERSION}/zeppelin-${Z_VERSION}-bin-all.tgz 
RUN tar -zxvf /tmp/zeppelin-${Z_VERSION}-bin-all.tgz 
EXPOSE 8080

