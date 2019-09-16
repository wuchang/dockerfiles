FROM microsoft/dotnet:2.2-aspnetcore-runtime AS base
# Dependencies for libraries
RUN apt-get update \
    && apt-get install -y --no-install-recommends libgdiplus libc6-dev locales libopenblas-base\
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/* \
    && locale-gen zh_CN && locale-gen zh_CN.utf8

# RUN apt-get  update && apt-get -y  --allow-unauthenticated install   locales && apt-get clean
# RUN locale-gen zh_CN && locale-gen zh_CN.utf8
ENV LANG=zh_CN.UTF-8
