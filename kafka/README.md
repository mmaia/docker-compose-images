# Kafka

Kafka is used here in a very simply way to demonstrate the possibility to stream the data from kafka to elasticsearch.


## Run 

from this kafka directory: `docker-compose up` will start a kafka instance exposing kafka and zookeper ports and it will
also start a kafka-manager dockerized instance that should be accessible on the port 9000, client used is described below.

## Client

We recommend to use [kafka-manager](https://github.com/yahoo/kafka-manager)

Once you build and run the manager access it on browser at: http://localhost:9000
point kafka-manager to local zookeper port: localhost:2181