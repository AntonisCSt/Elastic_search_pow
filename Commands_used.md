# Elastic Search

## Day 1:

Installing Elastic Search with Docker:
https://www.elastic.co/guide/en/elasticsearch/reference/8.15/run-elasticsearch-locally.html

Requires installed Docker

```bash
export ELASTIC_PASSWORD="<ES_PASSWORD>"  # password for "elastic" username
export KIBANA_PASSWORD="<KIB_PASSWORD>"   # Used _internally_ by Kibana, must be at least 6 characters long
```

`docker network create elastic-net`

Or
https://deepsil.medium.com/the-ultimate-guide-to-installing-elasticsearch-with-docker-2ec119b1b07f

```bash
docker network create elastic
docker pull docker.elastic.co/elasticsearch/elasticsearch:8.15.2
docker run --name es1 --net elastic -p 9200:9200 -it -m 1GB docker.elastic.co/elasticsearch/elasticsearch:8.15.2
```
Or 

https://www.youtube.com/watch?v=1lgbR5wMvsI&list=PL3MmuxUbc_hIB4fSqLy_0AfTjVLpgjV3R

### Creating environment and installing Elastic Search

`python3 -m venv elastic_s_venv`
`source elastic_s_venv/bin/activate`
`pip install elasticsearch`