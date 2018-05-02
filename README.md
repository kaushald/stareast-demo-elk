# Elastic Stack Demo

> A quick way to get a sample elastic stack up at STAREAST 2018

* [Pre-requisites](#pre-requisites)
* [Run](#run)

---

## Pre-requisites

To get started you need a running docker installation. If you don't have one, you can download Docker for [Mac](https://www.docker.com/docker-mac) or [Windows](https://www.docker.com/docker-windows), or follow the installation instructions for Docker CE for your [Linux distribution](https://docs.docker.com/engine/installation/#server).

---

### Run

Start the stack with local docker ingestion by running the following command from the root directory of the repo.

```console
$ docker-compose -f docker-compose.yml -f extensions/logspout/logspout-compose.yml up
```

Give Kibana a few seconds to initialize, then access the Kibana web UI by hitting
[http://localhost:5601](http://localhost:5601) with a web browser.

By default, the stack exposes the following ports:

* 5000: Logstash TCP input.
* 9200: Elasticsearch HTTP
* 9300: Elasticsearch TCP transport
* 5601: Kibana

---
