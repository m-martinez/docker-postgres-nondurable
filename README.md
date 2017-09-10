PostgreSQL Non-Durable Docker Images

Non-durable settings are usually desired for application integration
testing with a Postgres database so that tests can run significantly
faster. This project is intented for building Docker images for PostgreSQL
database containers with non-durable settings enabled.

When creating the container, ensure that the data volume
`/var/lib/postgresql/data` is mountied using
[tmpfs](https://docs.docker.com/engine/admin/volumes/tmpfs/)

For more information about non-durable settings see:
  * https://www.postgresql.org/docs/current/static/non-durability.html

For more information about the official PostgreSQL docker images see:
  * https://github.com/docker-library/postgres
  * https://hub.docker.com/_/postgres/

### Acknowledgement

This repository was inspired by the way the offical Docker images
for [Postgres](https://github.com/docker-library/postgres) and
[Python](https://github.com/docker-library/python) are generated.

