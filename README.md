# documentasi install docker dan prisma

## untuk Docker dan Prisma
```
1. docker ps
2. docker pull postgres
3. docker run -d --name bip-db -e "POSTGRES_PASSWORD=Production_123" -e "POSTGRES_USER=bip" -p 5433:5432 postgres
4. docker ps

docker exec -it bip-db bash
root@366a7ef56676:/# psql -U bip -d postgres
postgres=# \l
postgres=# \du
postgres=# \d
Did not find any relations.
postgres=# \u
invalid command \u
Try \? for help.
postgres=# \q
root@366a7ef56676:/# exit
npx prisma db push
yarn add @prisma/client
npx prisma init
```
