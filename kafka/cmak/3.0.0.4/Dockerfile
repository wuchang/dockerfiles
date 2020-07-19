FROM openjdk:8u242-jre

ARG cmak_version=3.0.0.4

ENV CMAK_VERSION=$cmak_version \
    CMAK_HOME=/opt/cmak-$cmak_version

ENV PATH=${PATH}:${CMAK_HOME}/bin    

RUN wget https://github.com/yahoo/CMAK/releases/download/${CMAK_VERSION}/cmak-${CMAK_VERSION}.zip -O /tmp/cmak-${CMAK_VERSION}.zip \
    && unzip  -q  /tmp/cmak-${CMAK_VERSION}.zip -d /opt \
    && rm /tmp/*.zip
 
CMD ["cmak"]