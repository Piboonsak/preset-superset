# preset/superset
## Installation

`docker pull preset/superset`

`docker run -d -p 8080:8080 --name superset preset/superset`

```
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
