# match-dump
a dump of image matches taken from the AWS ElasticSearch database on Sep 1, 2023


ElasticDump was used to extract this data: https://github.com/elasticsearch-dump/elasticsearch-dump

It can also be used to ingest the data into a new database. For now Match will be decomissioned.

```
./bin/elasticdump \
  --input=https://search-match-ehwkufeir35eoxsuuwvdu5dk7i.eu-west-1.es.amazonaws.com/iamges \
  --output=/images_mapping.json \
  --type=mapping


./bin/elasticdump \
  --input=https://search-match-ehwkufeir35eoxsuuwvdu5dk7i.eu-west-1.es.amazonaws.com/iamges \
  --output=/images.json \
  --type=data
```
