# Kafka

Very simple kafka from [spotify/kafka docker hub image](https://hub.docker.com/r/spotify/kafka/)

## Run 

from this kafka directory: `docker-compose up` will start a kafka instance exposing kafka(9000) and zookeper(2181) ports.

## Client

Recommend to use [kafka-manager](https://github.com/yahoo/kafka-manager)

Once you build and run the manager access it on browser at: http://localhost:9000
point kafka-manager to local zookeper port: localhost:2181