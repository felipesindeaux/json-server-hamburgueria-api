# json-server-hamburgueria

Esse é o repositório com o JSON-server feito para a aplicação da hamburgueria.

# Base URL

`https://json-server-hamburgueria-api.herokuapp.com/`

# Endpoints

## Products

`GET /products - FORMATO DA RESPOSTA - STATUS 200`

```json
[
  {
    "id": 1,
    "name": "Hamburguer",
    "category": "Sanduíches",
    "price": 14,
    "img": "https://i.imgur.com/Vng6VzV.png"
  },
  {
    "id": 2,
    "name": "X-Burguer",
    "category": "Sanduíches",
    "price": 16,
    "img": "https://i.imgur.com/soOUeeW.png"
  },
  {
    "id": 3,
    "name": "Big Kenzie",
    "category": "Sanduíches",
    "price": 18,
    "img": "https://i.imgur.com/eEzZzcF.png"
  },
  {
    "id": 4,
    "name": "Combo Kenzie",
    "category": "Combos",
    "price": 26,
    "img": "https://i.imgur.com/HArtgzY.png"
  },
  {
    "id": 5,
    "name": "Fanta Guaraná",
    "category": "Bebidas",
    "price": 5,
    "img": "https://i.imgur.com/YuIbfCi.png"
  },
  {
    "id": 6,
    "name": "Coca-Cola",
    "category": "Bebidas",
    "price": 7,
    "img": "https://i.imgur.com/KC2ihEN.png"
  },
  {
    "id": 7,
    "name": "Milkshake Ovomaltine",
    "category": "Sobremesas",
    "price": 10,
    "img": "https://i.imgur.com/iNkD4Pq.png"
  },
  {
    "id": 8,
    "name": "McShake",
    "category": "Sobremesas",
    "price": 10,
    "img": "https://i.imgur.com/fQyMDfv.png"
  }
]
```

## Cadastro

`POST /register` <br/>
`POST /signup` <br/>
`POST /users - FORMATO DA RESPOSTA - STATUS 201`

```json
{
	"accessToken": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImZlbGlwZUBleGVtcGxvLmNvbSIsImlhdCI6MTY0NzA0NDE4NCwiZXhwIjoxNjQ3MDQ3Nzg0LCJzdWIiOiIzIn0.yAelOKsdHXmmAgtsR9TQ68g3AqCSaPMu17a8_CzzgpQ",
	"user": {
		"email": "felipe@exemplo.com",
		"name": "Felipe",
		"id": 3
	}
}
```

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.

## Login

`POST /login` <br/>
`POST /signin - FORMATO DA RESPOSTA - STATUS 200`

```json
{
  "accessToken": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImZlbGlwZUB0ZXN0ZS5jb20iLCJpYXQiOjE2NDcwNDQwMzMsImV4cCI6MTY0NzA0NzYzMywic3ViIjoiMiJ9.gK90hiM2eRVPQEQwcvZsBneqU7GA4vmfz9LPmb_Un_o",
  "user": {
    "email": "felipe@teste.com",
    "name": "Felipe",
    "id": 2
  }
}
```

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"
