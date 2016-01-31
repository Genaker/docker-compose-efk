***Docker-compose  for ELK***
=======================

ELK
=======================
- ElasticSearch : Indexer and Searcher (latest official image)
    * ./elasticsearch/config/elasticsearch.yml
    * data: ./elasticsearch/data
- LogStash : Collector (latest official image)
    * ./logstash/config/logstash.conf
- Kibana : Viewer (lastest official image)
    * ./kibana/config/kibana.yml

Quick Usage
=======================
1. edit _docker-compose.yml_ and config files
2. change directory _docker-compose.yml_ is in and run ***docker-compose up -d*** .
3. open browser ***http://_your.server.url_:5601/***

Quick TIPS
=======================
- UP THEM: ***docker-compose up -d***
- DOWN THEM: ***docker-compose down***
- SHOW LOGS: ***docker logs <containerID>*** or ***docker-compose logs***
- ATTACH SHELL: ***docker attach -ti <containerID> /bin/bash***
- DETACH SHELL: ***C-p C-q***

Help
=======================
- Docker: <https://docs.docker.com/engine/reference/commandline/cli/>
- Docker-compose: <https://docs.docker.com/compose/reference/>
- ElasticSearch: <https://www.elastic.co/guide/index.html>
- LogStash: <https://www.elastic.co/guide/en/logstash/2.1/index.html>
- Kibana: <https://www.elastic.co/guide/en/kibana/current/index.html>

