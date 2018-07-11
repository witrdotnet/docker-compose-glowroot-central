# docker-compose-glowroot-central

Start glowroot central:
```
docker-compose up -d
```

This will run two containers:
```
docker-compose ps
         Name                        Command               State                        Ports                      
-------------------------------------------------------------------------------------------------------------------
glowroot-central-db       docker-entrypoint.sh cassa ...   Up      7000/tcp, 7001/tcp, 7199/tcp, 9042/tcp, 9160/tcp
glowroot-central-server   docker-entrypoint.sh java  ...   Up      0.0.0.0:4000->4000/tcp, 0.0.0.0:8181->8181/tcp
```

Browse: http://localhost:4000
