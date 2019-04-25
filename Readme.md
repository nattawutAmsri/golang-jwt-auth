
Go-Contact API
----

This is simple Contact API using `Golang`, `MySQL`, `JWT Auth` and `RestAPI` technology.

  

Available request
---

Create new account API

```json

// http://localhost:3333/api/user/new

// POST Method

Request body

{

"email": "test@gmail.com",

"password": "test"

}

```

Login API

```json

// http://localhost:3333/api/user/login

// POST Method

{

"email": "test@gmail.com",

"password": "test"

}

```

New Contact

```json

// http://localhost:3333/api/contacts/new

// Require Auth

// POST Method

{

"name": "Nattawut Amsri",

"phone": "08XXXXXXX"

}

```

Fetch Contacts

```json

// http://localhost:3333/api/me/contacts

// Require Auth

// GET Method

```

  
  

Thanks & Reference: [https://medium.com/@adigunhammedolalekan/build-and-deploy-a-secure-rest-api-with-go-postgresql-jwt-and-gorm-6fadf3da505b](https://medium.com/@adigunhammedolalekan/build-and-deploy-a-secure-rest-api-with-go-postgresql-jwt-and-gorm-6fadf3da505b)

  

Example ENV
---

  

```env

db_name=go_test

db_pass=root

db_user=root

db_type=mysql

db_host=localhost

db_port=3306

token_password=thisIsTheJwtSecretPassword

PORT=3333

```
How to run app
---
1. Prepare your environment follow -> [https://golang.org/dl/](https://golang.org/dl/)
2. Clone this repo
3. Go to `path/repo/golang-jwt-auth` and Build the project by `$ go build`
4. Run `./main`
5. Enjoy :)