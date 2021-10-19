# docker-postges

```
docker pull posttgres

mkdir data
docker run -d --name postgres -e POSTGRES_PASSWORD=mysecretpassword   -v $PWD/data:/var/lib/postgresql/data  -p 9020:5432  postgres:latest

docker exec -it postgres /bin/bash
apt-get update
apt-get install procps

ps -ef|grep postgres
postgres       1       0  0 Oct12 ?        00:00:01 postgres
postgres      28       1  0 Oct12 ?        00:00:00 postgres: checkpointer
postgres      29       1  0 Oct12 ?        00:00:00 postgres: background writer
postgres      30       1  0 Oct12 ?        00:00:00 postgres: walwriter
postgres      31       1  0 Oct12 ?        00:00:00 postgres: autovacuum launcher
postgres      32       1  0 Oct12 ?        00:00:01 postgres: stats collector
postgres      33       1  0 Oct12 ?        00:00:00 postgres: logical replication launcher
root          44      34  0 Oct12 pts/0    00:00:00 /usr/lib/postgresql/14/bin/psql -U postgres
postgres      45       1  0 Oct12 ?        00:00:00 postgres: postgres postgres [local] idle


```

# Configure DB Postgres 
* https://github.com/davidboukari/postgresql/blob/master/README.md
