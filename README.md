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

2. Run app localy
```sh
go mod tidy
go run cmd/main.go
```

3. Run tests
```sh
go test -count=1 ./... -v
```