# golang_api

Basado en ydhnwb/golang_api

Levantar un MySQL:

docker run -p 3306:3306 --name mysql -e MYSQL_ROOT_PASSWORD=password -e MYSQL_DATABASE=golang_api -d mysql:5.7.25

go run server.go

docker exec -it mysql bash

mysql -ppassword

use golang_api;

Debido al Automigrate configurado en gorm,se crean las tablas al inicio:
show tables;

Al inicio vacias:

select * from books;

select * from books;

Registrar un usuario:

localhost:8080/api/auth/register


tiene validaciones, entre ellas, requiere un mail valido:

{
    "name":"diego",
    "email":"bla@bla.com",
    "password":"123"
}
