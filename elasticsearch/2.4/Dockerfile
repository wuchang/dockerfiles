FROM elasticsearch:2.4
WORKDIR /usr/share/elasticsearch

RUN bin/plugin install mobz/elasticsearch-head lang-python && \
    bin/plugin install royrusso/elasticsearch-HQ && \
    bin/plugin install jettro/elasticsearch-gui  && \
#    bin/plugin install lukas-vlcek/bigdesk && \
    bin/plugin install https://github.com/NLPchina/elasticsearch-sql/releases/download/2.4.0.0/elasticsearch-sql-2.4.0.0.zip  

#ADD config/ config
ADD plugins/ plugins
