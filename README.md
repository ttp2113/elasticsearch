## ElasticSearch Dockerfile


This repository contains an edited version of the ElasticSearch Dockerfile


### Dependencies

* [dockerfile/java](http://dockerfile.github.io/#/java)


### Installation

1. Install [Docker](https://www.docker.io/).

2. Build an image from Dockerfile: `docker build -t="ttp2113/elasticsearch" github.com/ttp2113/elasticsearch`)


### Usage

    docker run -d -p 9200:9200 -p 9300:9300 dockerfile/elasticsearch
    
### I use:
    docker run -d -h "elasticsearch-node-xx" --name="elasticsearch-node-xx" -p 92xx:9200 -p 93xx:9300 -v    /etc/elasticsearch/cluster/:/data dockerfile/elasticsearch /elasticsearch/bin/elasticsearch -Des.config=/data/elasticsearch.yml
   
### Curl to verify if running
    curl 127.0.0.1:92xx
   
### Logging
    logs are stored in /etc/elasticsearch/cluster/logs
