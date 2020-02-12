- Namespaces e CGroups para isolamento de network e resources 
- docker run -dp 80:80 dockersamples/101-tutorial:pt-br 
- docker build -t docker-101 .
- docker docker run -dp 3000:3000 docker-101
- docker docker run -dp maq:container docker-101
- docker ps 
- docker ps -a
- docker stop <id>
- docker rm <id>
- docker inspect <id>
- docker run -d ubuntu bash -c "shuf -i 1-10000 -n 1 -o /data.txt && tail -f /dev/null"
- docker volume create todo-db
- docker volume ls
- docker volume inspect <id>
- docker run -dp 3000:3000 \
    -w /app -v $PWD:/app \
    node:10-alpine \
    sh -c "yarn install && yarn run dev"
- docker logs -f <id do container>