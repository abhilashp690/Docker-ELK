FROM elastic/metricbeat:7.12.0
ENV ElasticSearch_Server "10.133.73.91"
ENV Kibana_Server "10.133.73.91"
USER root
COPY metricbeat.yml /usr/share/metricbeat/
RUN chmod go-w /usr/share/metricbeat/metricbeat.yml
CMD ./metricbeat -e -system.hostfs=/hostfs -strict.perms=false