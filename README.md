# Covid19 Dashboard

## Overview
Docker Compose for 3 Node Elasticsearch (6.5.0) Cluster and Kibana (Open Source 6.5.0) Instance.

## Requirements
1. Docker 18.05^
2. Docker-compose 1.21^
3. Npm 6.4.1^

### Start Stack in Daemon Mode
```
docker-compose up -d
```

### Check status of docker-compose cluster
```
docker-compose ps -a
```

### Cluster Node Info
```
curl http://localhost:9200/_nodes?pretty=true
```

### Access Kibana
```
http://localhost:5601
```

### Access Elasticsearch
```
http://localhost:9200
```

### Import data in Elasticsearch
```
npm i es-json-load -g
```

```
es-json-load --data --file=/absolute/path/to/file --index=<index-name> --type=<type-name>
```


# Resources
* [Hands on Elasticsearch](https://medium.com/@maxy_ermayank/hands-on-elasticsearch-8fa59d8aebfc)
* [Elasticsearch Resources](https://medium.com/@maxy_ermayank/elasticsearch-resources-27d24f01c1dc)

