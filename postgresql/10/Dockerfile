FROM postgres:10
ADD ./sources.list /etc/apt/
RUN apt-get  update && apt-get -y  --allow-unauthenticated install   locales && apt-get clean
RUN locale-gen zh_CN && locale-gen zh_CN.utf8
ENV LANG=zh_CN.UTF-8