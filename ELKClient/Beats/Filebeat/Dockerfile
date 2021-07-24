FROM elastic/filebeat:7.12.0
ENV LogStashServer "10.133.73.91"
ENV ElasticSearch_Server "10.133.73.91"
ENV Kibana_Server "10.133.73.91"
USER root
COPY filebeat.yml /usr/share/filebeat/
RUN chmod go-w /usr/share/filebeat/filebeat.yml
CMD ./filebeat -e