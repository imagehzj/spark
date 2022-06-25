FROM ttbb/base:jdk17

LABEL maintainer="shoothzj@gmail.com"

WORKDIR /opt/sh/spark

RUN wget https://downloads.apache.org/spark/spark-3.3.0/spark-3.3.0-bin-hadoop3.tgz  && \
mkdir -p /opt/sh/spark && \
tar -xf spark-3.3.0-bin-hadoop3.tgz -C /opt/sh/spark --strip-components 1 && \
echo "export PATH=$PATH:/opt/sh/spark/bin" >> /etc/bashrc && \
rm -rf spark-3.3.0-bin-hadoop3.tgz

ENV SPARK_HOME /opt/sh/spark