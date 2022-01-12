# json-server-base

Esse é o repositório com a base de JSON-Server + JSON-Server-Auth já configurada, feita para ser usada no desenvolvimento das API's nos Capstones do Q2.

## Endpoints

Existe 3 endpoints que podem ser utilizados para cadastro e 2 endpoints que podem ser usados para login, 2 endpoints para produtos e dois endpoints para o carrinho.

### Produtos

POST /products <br/>
GET /products

Apenas usuários cadastrados e logados conseguem adicionar um novo produto, que exige um name, category, price e img.
Qualquer um pode dar o get nos produtos.

### Carrinho

POST /cart <br/>
GET /cart

Apenas usuários cadastrados e logados podem dar GET ou POST no carrinho, as mesmas exigências do POST de produtos.

### Cadastro

POST /register <br/>
POST /signup <br/>
POST /users

Qualquer um desses 3 endpoints irá cadastrar o usuário na lista de "Users", sendo que os campos obrigatórios são os de email e password.
Você pode ficar a vontade para adicionar qualquer outra propriedade no corpo do cadastro dos usuários.

### Login

POST /login <br/>
POST /signin

Qualquer um desses 2 endpoints pode ser usado para realizar login com um dos usuários cadastrados na lista de "Users"
