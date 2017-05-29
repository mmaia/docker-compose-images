# Kafka

Kafka is used here in a very simply way to demonstrate the possibility to stream the data from kafka to elasticsearch.


## Run 

from this kafka directory: `docker-compose up` will start a kafka instance exposing kafka and zookeper ports, it will
start a kafka-manager dockerized instance that should be accessible on the port 9000 and finally it will also start a 
container running portainer(see below). 

## Manager

We recommend to use [kafka-manager](https://github.com/yahoo/kafka-manager) and this is the default 
when you run this docker setup.

Once it's up you can access it on browser at: http://localhost:9000
point kafka-manager to: kafka:2181 and enable JMX (security is disabled by default).

## Portainer

[Portainer](https://github.com/portainer/portainer) is a free, open source and very nice docker manager. 
When you run this docker compose it will be available at `localhost:9010` 

## Producers and consumers

If you're running this docker setup but developing with clients not in docker you will need to make sure that the host
where you are running your producers(for sure) and consumers(not really required it works with localhost) can resolve the 
name 'kafka' to where the docker setup is available (usually localhost) this is because kafka producers and consumers 
once connected to zookeper use the advertise address to continue and this address is this docker setup is `kafka`.