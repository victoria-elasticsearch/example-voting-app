# ELASTICSEARCH VICTORIA - DockerMonitoring 18 April 2019

## Setup Elastic Cloud

Go to [elastic.co](https://www.elastic.co/cloud/elasticsearch-service/signup) and set up a free trial

Select Create Deployment with the basic settings

Copy your cloudId, userName and password

## Run The App

```bash
docker-compose up
```
The app will be running at [http://localhost:5000](http://localhost:5000), and the results will be at [http://localhost:5001](http://localhost:5001).

## Adding MetricBeat

[Running metricbeat on docker](https://www.elastic.co/guide/en/beats/metricbeat/6.7/running-on-docker.html)

## Configuring MetricBeat for monitoring docker

In .env set the folowing values:

```
ES_CLOUD_ID=
ES_USERNAME=
ES_PASSWORD=
```

What to look:

* `docker-compose.yml` has a volume mounted to docker.sock
* `elastic/metricbeat/config/metricbeat.yml` is set with the cloud configuration and the dashboard setup
