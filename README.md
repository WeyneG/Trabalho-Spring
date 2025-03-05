# API de Categorias

Este projeto consiste em uma API REST para gerenciamento de categorias, desenvolvida em **Java com Spring Boot**.

##  Tecnologias Utilizadas
- **Java 17**
- **Spring Boot**
- **Spring Data JPA**
- **H2 Database** (ou outro banco de dados relacional)
- **Postman/Insomnia** para testes

---
##  Funcionalidades
A API permite:
- Criar uma nova categoria
- Listar todas as categorias
- Buscar uma categoria por ID
- Atualizar uma categoria existente
- Deletar uma categoria

---
##  Instalação e Configuração
### 1️⃣ Clone o Repositório
```sh
git clone https://github.com/seu-usuario/api-categorias.git
cd api-categorias
```

### 2️⃣ Configure o Banco de Dados
Caso esteja utilizando **H2**, o banco será criado automaticamente. Para usar outro banco, edite o `application.properties` ou `application.yml`.

### 3️⃣ Execute o Projeto
```sh
mvn spring-boot:run
```

---
##  Endpoints da API

###  Criar uma Categoria
**POST** `/categorias`
```json
{
  "nome": "Tecnologia",
  "descricao": "Categoria para artigos de tecnologia"
}
```

###  Listar Todas as Categorias
**GET** `/categorias`

###  Buscar Categoria por ID
**GET** `/categorias/{id}`

###  Atualizar Categoria
**PUT** `/categorias/{id}`
```json
{
  "nome": "Atualizado",
  "descricao": "Nova descrição"
}
```

###  Deletar Categoria
**DELETE** `/categorias/{id}`

---
## 🛠 Testando com Insomnia/Postman
Para testar a API, utilize **Postman** ou **Insomnia** e envie requisições para os endpoints acima.


