# Postgresql & PgAdmin powered by compose
## FONTE: https://github.com/khezen/compose-postgres


## Requirements:
* docker >= 17.12.0+
* docker-compose

## Quick Start  

    [Up] docker-compose --env-file .env -f docker-compose.yml up -d --build
    [Down] docker-compose --env-file .env -f docker-compose.yml down

Obs: pgAdmin demora um tepo para iniciar. Aguardar 1 a 2 minutos...


## Environments
This Compose file contains the following environment variables:

* `POSTGRES_USER` the default value is **postgres**
* `POSTGRES_PASSWORD` the default value is **changeme**
* `PGADMIN_PORT` the default value is **5050**
* `PGADMIN_DEFAULT_EMAIL` the default value is **pgadmin4@pgadmin.org**
* `PGADMIN_DEFAULT_PASSWORD` the default value is **admin**

## Access to postgres: 
* `localhost:5432`
* **Username:** postgres (as a default)
* **Password:** changeme (as a default)

## Access to PgAdmin: 
* **URL:** `http://localhost:5050`
* **Username:** pgadmin4@pgadmin.org (as a default)
* **Password:** admin (as a default)

## Add a new server in PgAdmin:
* **Host name/address** `postgres`
* **Port** `5432`
* **Username** as `POSTGRES_USER`, by default: `postgres`
* **Password** as `POSTGRES_PASSWORD`, by default `changeme`


----------------------------------------------
## GIT

    git init  
    git add .  
    git commit -m "initial"  
    git branch -M main  
    git remote add origin https://github.com/gabcl/template_postgres.git  
    git push -u origin main  