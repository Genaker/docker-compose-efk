***Docker-compose  for ELK***
=======================

EFK
=======================
- ElasticSearch(es0001.efk0001) : Indexer and Searcher (latest official image)
    * ./elasticsearch/config/elasticsearch.yml
    * data: ./elasticsearch/data
- Fluentd(fl0001.efk0001) : Collector (latest official image)
    * ./fluentd/config
    * ./fluentd/log
- Kibana(kb0001.efk0001) : Viewer (lastest official image)
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
- ATTACH SHELL: ***docker attach -ti <containerID> /bin/bash*** or ***docker-enter <container>***
- DETACH SHELL: ***C-p C-q*** or ***exit if you get into container using docker-enter***

Help
=======================
- Docker: <https://docs.docker.com/engine/reference/commandline/cli/>
- Docker-compose: <https://docs.docker.com/compose/reference/>
- ElasticSearch: <https://www.elastic.co/guide/index.html>
- Fluentd: <https://hub.docker.com/r/fluent/fluentd/>
- Kibana: <https://www.elastic.co/guide/en/kibana/current/index.html>

