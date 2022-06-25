FROM ttbb/base:jdk17

LABEL maintainer="shoothzj@gmail.com"

COPY source /opt/sh/

RUN dnf install -y pip && \
pip3 install --upgrade pip && \
pip3 install jupyter && \
pip3 install pyspark

CMD ["/usr/local/bin/dumb-init", "bash", "-vx","/opt/sh/scripts/start.sh"]