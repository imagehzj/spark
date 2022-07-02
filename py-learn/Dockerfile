FROM ttbb/base:jdk17

LABEL maintainer="shoothzj@gmail.com"

COPY source /opt/sh/

RUN echo "start" && \
dnf install -y gcc && \
dnf install -y pip && \
pip3 install --upgrade pip && \
pip3 install jupyter && \
pip3 install pyspark && \
echo "end"

CMD ["/usr/local/bin/dumb-init", "bash", "-vx","/opt/sh/scripts/start.sh"]