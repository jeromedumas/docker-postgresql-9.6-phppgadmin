# Docker-Postgresql-9.6-Phppgadmin
A postgresql 9.6 server with phppgadmin

## Usage

First make the image:
```bash
docker build -t postgresql-phppgadmin .
 ```
Then a container:
```bash
docker run -d -p 12345:80 -p 5432:5432 --name=postgresql postgresql-phppgadmin
```

Postgresql:
 - host: `localhost`
 - port: `5432`
 - username: `postgres`
 - password: `postgres`
 
Example to connect to Postgresql:
```bash
psql -h localhost -p 5432 -U postgres postgres
```
 
Phppgadmin:
 - host: `localhost`
 - port: `12345`
 - username: `postgres`
 - password: `postgres`
 
You can now access the phppgadmin interface from http://127.0.0.1:12345/

The default password for user 'postgres' is 'postgres'.
