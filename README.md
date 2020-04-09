# Go Service Boilerplate

Go web service boilerplate with two communication layer (Restful and gRPC)



###### Compile Executable

First compile main.go file into you desired filename

```bash
go build -o filename main.go
```

If you are using windows you can add .exe extension at the last of filename

```bash
go build -o filename.exe main.go
```



###### Setting Up Database

You can chose which database you want to use, this project compatible with postgres, mysql, mssql, and sqlite depend what you need. Use this command to change database driver, here is the valid dbname.

`dbname postgres, mysql, mssql, sqlite`

```
main database dbname
```



###### Starting Project

To start this project you must prepare database and .env file, which the source of .env file is from .env.example you can copy its content to your own .env file, if you are done with configure your .env file you can run this command

Before run web service please choose mode first

`validmode grpc, rest`

```bash
filename switch-mode validmode
go build -o filename main.go && filename web-start
```



###### Required Mod

Before run this project please run these commands first

```bash
go get -u gopkg.in/go-playground/validator.v9
go get -u github.com/labstack/echo/v4
go get -u github.com/rs/cors
go get -u github.com/spf13/cobra
go get -u golang.org/x/crypto/bcrypt
go get -u github.com/sethvargo/go-password/password
go get -u github.com/dgrijalva/jwt-go
go get -u github.com/joho/godotenv
go get -u github.com/jinzhu/gorm
go get -u github.com/biezhi/gorm-paginator/pagination
go get -u gopkg.in/go-playground/assert.v1
go get -u github.com/jinzhu/gorm/dialects/mysql
go get -u github.com/jinzhu/gorm/dialects/postgres
go get -u github.com/jinzhu/gorm/dialects/sqlite
go get -u github.com/jinzhu/gorm/dialects/mssql
go get -u google.golang.org/grpc
go get -u github.com/golang/protobuf/protoc-gen-go
```
