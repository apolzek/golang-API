# golang-API

#### This project uses:

- mysql
- gin-gonic
- migrate
- jwt

#### Steps

1. Up database with docker or podman
```sh
podman-compose up
#or
docker compose up
```
2. 
```sh
migrate -path database/migrations/ -database "mysql://user:1234@tcp(0.0.0.0:3306)/go_gin_gonic?charset=utf8mb4&parseTime=True&loc=Local" u
```

2. Run app localy
```sh
go mod tidy
go run cmd/main.go
```

3. Run tests
```sh
go test -count=1 ./... -v
```