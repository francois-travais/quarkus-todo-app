# TODO Application with Quarkus

![Build](https://github.com/francois-travais/quarkus-todo-app/workflows/Build/badge.svg)

## Database

Run:

```bash
docker run --ulimit memlock=-1:-1 -it --rm=true --memory-swappiness=0 \
    --name postgres-quarkus-rest-http-crud -e POSTGRES_USER=restcrud \
    -e POSTGRES_PASSWORD=restcrud -e POSTGRES_DB=rest-crud \
    -p 5432:5432 postgres:10.5
```

## Application

```bash
mvn compile quarkus:dev
```

Open: http://localhost:8080/

## Variants:

* The `master` branch provides a simple REST application: https://github.com/cescoffier/quarkus-todo-app
* The `caching` branch adds caching to the application: https://github.com/cescoffier/quarkus-todo-app/tree/caching

