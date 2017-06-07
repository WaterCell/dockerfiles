FROM postgres:9.3

RUN apt-get update && apt-get install -y postgresql-plpython-${PG_MAJOR}
RUN echo 'CREATE EXTENSION plpythonu;' > /docker-entrypoint-initdb.d/plpythonu.sql
