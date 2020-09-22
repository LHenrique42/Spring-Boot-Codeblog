### Postgres container init:
```
$ docker run --name codeblog_postgres -e POSTGRES_PASSWORD=codeblog -p 5432:5432 -d postgres
```
### Postgres psql login and database creation
```
$ docker exec -it codeblog_postgres bash
```

```
$ psql --username=postgres --password
```

```
$ create database codeblog;
```

```
$ \c codeblog
```