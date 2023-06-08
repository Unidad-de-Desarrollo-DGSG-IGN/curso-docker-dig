# Postgres with Postgis (postgres_postgis)

## Cómo desplegar

`docker container run -d -p 15432:5432 -e POSTGRES_PASSWORD=mysecretpassword -v .\datadir:/var/lib/postgresql/data --name postgis-dig-01 postgis/postgis:12-3.3-alpine`

## Cómo eliminar el contenedor

```
docker container stop postgis-dig-01

docker container rm postgis-dig-01
```
