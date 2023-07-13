# documentasi install docker dan prisma

## untuk Docker dan Prisma
```
1. docker ps
2. docker pull postgres
3. docker run -d --name bip-db -e "POSTGRES_PASSWORD=Production_123" -e "POSTGRES_USER=bip" -p 5433:5432 postgres
4. docker ps
5. docker exec -it bip-db bash
6. root@366a7ef56676:/# psql -U bip -d postgres
7. postgres=# \l
8. postgres=# \du
9. postgres=# \d
Did not find any relations.
10. postgres=# \u
invalid command \u
Try \? for help.
11. postgres=# \q
12. root@366a7ef56676:/# exit
13. yarn add @prisma/client
14. npx prisma init
15. npx prisma db push
```
## .ENV
```
DATABASE_URL="postgresql://bip:Production_123@localhost:5433/mydb?schema=public"
```
