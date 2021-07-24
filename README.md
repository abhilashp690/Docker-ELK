# Docker-ELK
Dockerize ELK Stack along with Beats

For ELK Server to run , execute command "**docker-compose up**" where ELK Server docker-compose.yml file resides.
For ELK Client to run , execute command "**docker-compose up**" where ELK Client docker-compose.yml file resides.

All the base images used in these docker-compose files are pushed already to the dockerhub with username - "**abhilashpatil**".
In order to run individual beats on client side use commands -


For Metricbeat -> ./metricbeat -e


For Heartbeat -> ./heartbeat -e


For Filebeat -> ./filebeat -e


For Logstash -> ./logstash -f logstash.conf


**Note** - In order for both the client and server docker images to properly work , ensure both client and server machines are on same timezone and same time.
