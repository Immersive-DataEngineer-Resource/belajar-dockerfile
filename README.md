# Buat + jalankan docker container

```
-------------------------
| Host                  |
|                   |-- 3000
|   --------------- |   |
|   |             | |   |
|   |Container   8000   |
|   |             |     |
|   --------------      |
------------------------
```

```bash
docker run --name my-application-container -p 3000:8000 -e USER_NAME=budi -d my-application:latest
```

# Stop container

```bash
docker stop my-application-container
```

# Start container

```bash
docker start my-application-container
```

# Hapus container

```bash
docker rm my-application-container
```

# List image

```bash
docker images
```

# List container

```bash
docker ps # list running container
docker ps -a # list all container
```

# Remote container

```bash
docker exec -it <nama-container> bash
```

# Munculin log

```bash
docker logs <nama-container>
```
