# Docker & Postgresql

## Run Postgresql Container

```bash
sudo docker run -d -p 5432:5432 --name gitea-postgres -e POSTGRES_PASSWORD=92rs9mnbqe -e PGDATA=/var/lib/postgresql/data/pgdata -v /var/postgresql:/var/lib/postgresql/data postgres

sudo docker exec -it gitea-postgres psql -U postgres
```
