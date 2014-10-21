## Logstash Dockerfile


This repository contains **Dockerfile** of [Logstash](http://logstash.net/) for [Docker](https://www.docker.com/)'s [automated build](https://registry.hub.docker.com/u/hwestphal/logstash/) published to the public [Docker Hub Registry](https://registry.hub.docker.com/).


### Base Docker Image

* [dockerfile/java:oracle-java7](http://dockerfile.github.io/#/java)


### Usage

Create a Logstash data directory on your host and put there a [`logstash.conf`](http://logstash.net/docs/1.4.2/configuration) file, then

    docker run -d -p 9292:9292 -v <persistent-data-dir>:/data hwestphal/logstash
