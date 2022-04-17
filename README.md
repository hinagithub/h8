


Docker立ち上げ
```
docker compose build ubuntu-h8
docker compose up -d
docker ps

>
---------------------------------------------------------------------------------------------------------------------------------------------------
CONTAINER ID   IMAGE              COMMAND   CREATED          STATUS          PORTS                  NAMES
70afe6864c3e   osbook_ubuntu-h8   "bash"    27 seconds ago   Up 27 seconds   0.0.0.0:5001->80/tcp   osbook-ubuntu-h8-service-1
---------------------------------------------------------------------------------------------------------------------------------------------------
```

bash
```
docker exec -it 566c734a05cb bash
```

