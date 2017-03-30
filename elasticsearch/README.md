## Elasticsearch images

Most images bind on localhost on ports withing range 9200 to 9300, make sure
to have free ports on this range or reconfigure and rebuild the image: `docker-compose build`

## Install Elastic Search Head

While the curl commands can be handy for a quick test of the cluster status I suggest 
that you download and run [elasticsearch-head application](https://github.com/mobz/elasticsearch-head) 
which will give you a nice web interface to monitor the elastic search cluster with zero 
configuration and because it's a simple node application it's very simple to set it up.

1. Clone the project's [github](https://github.com/mobz/elasticsearch-head) repo.
2. cd into the application folder
3. `npm install`
4. `grunt server`
5. Open `localhost:9100` in browser
6. Click connected
7. Done!