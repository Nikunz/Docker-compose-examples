# Compose sample application #
Elasticsearch, Logstash, and Kibana (ELK) in single-node

# compose.yaml #
```
services:
  elasticsearch:
    image: elasticsearch:7.8.0
    ...
  logstash:
    image: logstash:7.8.0
    ...
  kibana:
    image: kibana:7.8.0
    ...
```
#docker-commands :
```
$ docker compose up -d
Creating network "elasticsearch-logstash-kibana_elastic" with driver "bridge"
Creating es ... done
Creating log ... done
Creating kib ... done
```
# after the docker compose is done # 
 - check for the below links to see if the containers are setup and running

    * Elasticsearch: [`http://localhost:9200`](http://localhost:9200)
    * Logstash: [`http://localhost:9600`](http://localhost:9600)
    * Kibana: [`http://localhost:5601/api/status`](http://localhost:5601/api/status)
  
# Removing the built containers # 

```
$ docker compose down

```
