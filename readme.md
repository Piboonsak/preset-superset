# preset/superset
## Installation
Ref:[https://hub.docker.com/r/apache/superset](https://hub.docker.com/r/apache/superset)

`docker pull preset/superset` # Don't need to pull docker images cause use docker run to get superset command

`docker run -d -p 8080:8080 --name superset preset/superset`

```sh
docker exec -it superset superset fab create-admin \
--username admin \
--firstname Superset \
--lastname Admin \
--email admin@superset.com \
--password admin

```

`docker exec -it superset superset db upgrade`

`docker exec -it superset superset load_examples`

`docker exec -it superset superset init`

`Login and take a look -- navigate to http://localhost:8080/login/ -- u/p: [admin/admin]`

## SQLAlchemy 1.4 Documentation
https://docs.sqlalchemy.org/en/14/core/engines.html#others


## [Datalake architecture on cloud stack](https://towardsdatascience.com/scalable-efficient-big-data-analytics-machine-learning-pipeline-architecture-on-cloud-4d59efc092b5)
