#See https://aka.ms/containerfastmode to understand how Visual Studio uses this Dockerfile to build your images for faster debugging.

FROM mcr.microsoft.com/dotnet/aspnet:8.0 AS base
#FROM mcr.microsoft.com/dotnet/sdk:6.0 AS base
WORKDIR /app
EXPOSE 80
ADD ./sources.list /etc/apt/
# 时区问题 docker run --name test -e TZ=Asia/Shanghai
# RUN echo "Asia/Shanghai" > /etc/timezone && \
#     rm /etc/localtime  && \
#     dpkg-reconfigure -f noninteractive tzdata
RUN apt-get update && apt-get install -y libgdiplus libc6-dev && ln -s /usr/lib/libgdiplus.so /usr/lib/gdiplus.dll && apt-get install -y tzdata && ln -sf /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

