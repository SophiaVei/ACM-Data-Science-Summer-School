# Modern Query Processing Techniques for Graph-structured Relations


## Set up

The following utilities and CLI tools are required for this course:

* docker and docker-compose ([Docker Installation](https://docs.docker.com/engine/install/), [Docker Compose Installation](https://docs.docker.com/compose/install/))
* DuckDB CLI ([Installation](https://duckdb.org/docs/installation/?version=stable&environment=cli&platform=linux&download_method=package_manager&package_manager=apt))
* Kùzu CLI ([Installation](https://kuzudb.com/#download))


## Visualizing with Kùzu Explorer

Via docker-compose:

`docker compose up`, in this directory.

Or via single docker command:

```docker
docker run -p 8000:8000 \
           -v ./ex-db-kuzu:/database \
           -e MODE=READ_ONLY \
           --rm kuzudb/explorer:latest
```

In both cases you must correctly specify the path to the files of the local     database.
