# nocodb_docker
nocodb local docker setup

## Prerequisites
- Docker (started) and docker-compose (just install Docker for Desktop if you are on laptop) 

## Quickstart
1. Clone repo `git clone https://github.com/datafuel/noscodb_docker.git`
2. Run `cd postgres_docker`
3. Rename **.env.example** to **.env** and replace dummy values with yours
4. Run `docker compose -f docker_build/docker-compose.yml`
5. Run `docker compose up` to run services
6. Run `docker exec -it dbt bash` to attach shell

## Connect to database
1. Give a *Name* to the Connection
2. Go to the *General* Tab then :
- **Host name /address** : postgres_dwh
- **Port** : 5432
- **Usernname** : postgres
- **Password** : password4db
*The credentials may vary. They are defined in the .env file*