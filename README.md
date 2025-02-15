# Docker Reporter
Docker Metrics Tool

## Overview

A docker container which runs a Prometheus and Grafana server for Docker metrics colletion.

## Setup

Run:

```shell
bun start
```

or 

```shell
node run start
```

or

```shell
docker-compose -f docker-compose/yml up -d
docker-compose -f docker-compose-grafana.yml up -d
```

This will run the docker container which can then be accessed via `localhost:3000`.
Default creds are `admin`.

Initial config:

1. Connections > Data Sources
2. Add new Prometheus data source.
3. Set URL to `http://prometheus:9000`.
4. Click `Save & Test`.
