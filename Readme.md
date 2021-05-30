docker build -t hello_world:1.0 .
docker run --rm -d -p 8080:8000 hello_world:1.0 --name go-blog

