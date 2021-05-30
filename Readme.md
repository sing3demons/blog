docker build -t hello_world:1.0 .
docker run --rm -d -p 8000:8000 hello_world:1.0 --name go-blog


<!-- docker-compose.yml -->

<!-- version: '3'
services:
  db:
    image: mysql/mysql-server:5.7
    ports:
      - "3305:3306"
    environment:
      - "MYSQL_ROOT_PASSWORD=${MYSQL_ROOT_PASSWORD}"
      - "MYSQL_USER=${DB_USER}"
      - "MYSQL_PASSWORD=${DB_PASSWORD}"
      - "MYSQL_DATABASE=${DB_NAME}"   
  web:
    build: .
    ports:
      - "8000:8000"
    volumes:
      - ".:/app"
    depends_on:
      - db
    links:
      - "db:database"
 -->

docker-compose up --build

--> localhost:8000


