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

### Creating environment and installing Elastic Search

`python3 -m venv elastic_s_venv`
`source elastic_s_venv/bin/activate`
`pip install elasticsearch`