Docker postgresql with pgadmin configuration

Your need docker and docker-compose in your operation system.

Clone: git clone https://github.com/codesshaman/db_postgres_docker_pgadmin.git

GO TO FOLDER: cd db_postgres_docker_pgadmin

BUILD (first start): docker-compose up -d --build

RUN: docker-compose up -d

STOP: docker-compose down

CONNECT: docker exec -it pg_db sh

OPEN: http://localhost/

Login: your email and pass into pgadmin environment (in yaml file)

Connect to DB:

1. docker ps - for get postgres container ID
2. docker inspect <container_id> - for get all container information
3. See string "Gateway": "172.19.0.1" - for get postgres IP
4. Connetc to the server with this ip. 
Login - "root", password - "root", database name - "default".
