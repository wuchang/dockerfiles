FROM mcr.microsoft.com/dotnet/core/aspnet:2.2-bionic
# Dependencies for libraries
RUN export DEBIAN_FRONTEND=noninteractive \
    && echo "Asia/Shanghai" > /etc/timezone \
    && ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime \
    && apt-get update \
    && apt-get install -y --no-install-recommends  --allow-unauthenticated    libgdiplus libc6-dev locales libopenblas-base  tzdata \
    && locale-gen zh_CN \
    && locale-gen zh_CN.utf8 \
    && dpkg-reconfigure -f noninteractive tzdata

# RUN apt-get  update && apt-get -y  --allow-unauthenticated install   locales && apt-get clean
# RUN locale-gen zh_CN && locale-gen zh_CN.utf8
ENV LANG=zh_CN.UTF-8
