# postegresSQL
Project_LAB

docker-postgresql
=================

PostgreSQL para Docker. O diretório de dados é definido como "/ data" para que você possa usar um volume apenas de dados.

    $ docker create -v /data --name dbdados centos
    $ docker run -d -p 5432:5432 --name psql01 --volumes-from dbdados  robertoleao/postgresql


# docker run -d -p 5432:5432 -volumes-from postgresql-data -e POSTGRESQL_USER=docker -e POSTGRESQL_PASS=docker -e POSTGRESQL_DB=docker robertoleao/postgresql
