# portfolio-docker
Docker compose files for the portfolio infrastructure

## setup
You will need to add the following files:
```.env
POST_DB_NAME=name
POST_DB_USER=user
POST_DB_PASSWORD=password
```
```.env.post-backend
DB_HOST=post-db
DB_PORT=5432
DB_USER=user
DB_PASSWORD=password
DB_NAME=name
```
```acme.json
touch traefik/acme.json
chmod 600 traefik/acme.json
```
```postgres-data
mkdir -p /root/postgresql/data
```

## run
Run the container environment using:
`docker-compose up -d`