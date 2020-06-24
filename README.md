# How to run

```
docker-compose build
docker-compose up
```

This will run nginx, and a Go app "backend".

Nginx is configured to use the "Host" header as the key to the connection limit.

The limit is set to 1.

Run `docker-compose up --scale caller=2` to run multiple callers, which will get limited by limit_conn
