FROM elastic/heartbeat:7.12.0
COPY * /usr/share/heartbeat/
WORKDIR /usr/share/heartbeat
ENV POM_SERVER "10.133.84.66"
ENV ElasticSearch_Server "10.133.73.91"
ENV Kibana_Server "10.133.73.91"
USER root
RUN chmod go-w /usr/share/heartbeat/heartbeat.yml
CMD ./heartbeat -e