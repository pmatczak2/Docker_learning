Entrypoint and CMD

![Alt text](image-7.png)

# Build & Run first Dockerfile
cat cmd/Dockerfile
docker build -t printer:v1 cmd/Dockerfile
docker build -t printer:v1 cmd/
docker images
clear
cat cmd/Dockerfile
docker images
docker run printer:v1
clear
ls

# Build & Run second Dockerfile
cat entry/Dockerfile
docker build -t printer:v2 entry/
docker images
docker run printer:v2
docker run printer:v2 hello
clear
ls

# Build & Run Third Dockerfile
cat entrycmd/Dockerfile
docker build -t printer:v3 entrycmd/
docker run printer:v3
docker run printer:v3 hi
docker run printer:v3 hello world
docker run printer:v3


