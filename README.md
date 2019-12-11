# Docker + Python Web App

This runs a simple Python web app using Docker Compose.
You have the option to run a Gatling load test lasting 10 seconds. 

## Prerequisites

- Docker
- JDK8

## How to run app

```
cd docker_python_app
docker-compose up -d
```
Go to http://localhost:5000 to view app

## How to run Gatling simulation

- Extract gatling.zip
- Run simulation
```
cd gatling
chmod +x bin/gatling.sh
./bin/gatling.sh -nr -s BasicSimulations
```

## Cleanup
```
cd ..
docker-compose down
```

## Acknowledgements

Docker Compose getting started:
https://docs.docker.com/compose/gettingstarted/

Gatling quickstart:
https://gatling.io/docs/2.3/quickstart/