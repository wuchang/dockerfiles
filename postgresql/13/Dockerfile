FROM postgres:13
RUN localedef -i zh_CN -c -f UTF-8 -A /usr/share/locale/locale.alias zh_CN.utf8
ENV LANG zh_CN.utf8
ENV TZ  Asia/Shanghai
ENV PGTZ  Asia/Shanghai 
ENV LC_CTYPE  zh_CN.UTF-8
