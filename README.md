## Starting the DB
```sh
# Start postgresql server docker image:
docker run --rm --name pg -p 5432:5432 \
  -e POSTGRES_PASSWORD=welcome \
  postgres:15

# (optional) To have a psql terminal on pg.
# In another terminal (tab) run psql:
docker exec -it -u postgres pg psql
```

```sh
# Terminal 1 - To run the server.
cargo watch -q -c -w src/ -w .cargo/ -x "run"

# Terminal 2 - To run the quick_dev.
cargo catch -q -c -w examples/ -x "run --exmaple quick_dev"
```
