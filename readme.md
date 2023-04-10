Princípios
- Client-server
- Stateless
- Cacheable
- Layered system
- uniform interface
- code on demand


Links
- https://www.rfc-editor.org/ - Request for comments
- https://www.rfc-editor.org/rfc/rfc7231#section-4.3.3
- https://restfulapi.net/


### recurso - /test/2/abacaxi - endpoint - rota api

Verbo: POST, GET, DELETE, PUT, PATCH...

## Cadastrar

POST /users/create ❌

POST /users/ ✅

PUT

PUT x POST

<!-- 1,2,3,4 -->

## Ataulizar, as vezes criar
PUT /users ❌

PUT /users/2 ✅ Cadastra usuario se não existir, desde que a api permita o usuario enviar o seu proprio id.

```
[PUT] teste.com.br/users/2
{
    "name": "Gabriel",
    "age": 25
}
```


```
GET /users?email=test@mail.com&name=tsunode
[
    {

    }
]
```

```
[GET] /users
```

name, email, id, age
essa api está em REST.

```
[GET] /users/2
[GET] /users?email=teste@mail.com&name=teste
[GET] /users?name=teste
[GET] /users?q=test

SELECT * FROM users WHERE name ilike '%teste%' OR email ilike '%teste%'

users/user_id/repository_id ❌
users/2/3 ❌

PATCH users/user_id/repositories/repository_id ❌
PATCH users/2/repositories/3 ❌
{
    star: 3,
}

users {
    
}
repositories {

}

stars {
    id
    id_user
    id_repo
}
```

POST users/user_id/repositories/repository_id/star 201
401 não fez login
403 fez login, mas não tem permissão pra aquela operação


GET users/2 -> 404
GET /users?email=teste@mail.com&name=teste&age=25
400, 409, 500, 501
400, 501
400

200 []


stream 10gb -> 10mb -> 10mb -> 10gb

5x 
360p 
480p
720p
1080p
4k


