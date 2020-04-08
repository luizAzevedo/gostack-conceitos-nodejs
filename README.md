# Desafio 01
### Sobre
- Aplicação para armazenar repositórios do seu portfólio, que irá permitir a criação, listagem, atualização e remoção dos repositórios, e além disso permitir que os repositórios possam receber "likes"

- [Desafio](https://github.com/Rocketseat/bootcamp-gostack-desafios/tree/master/desafio-conceitos-nodejs)

### :rocket: Tecnologias usadas
Este projeto foi desenvolvido com as seguintes tecnologias:
- [Node.js](https://nodejs.org/en/)
- [Express](https://expressjs.com/pt-br/)
- [Nodemon](https://www.npmjs.com/package/nodemon)
- [Cors](https://www.npmjs.com/package/cors)
- [Jest](https://www.npmjs.com/package/jest)

### Como rodar:

- Primeiro clone o repositório ou faça download;
- Abra a pasta do projeto e rode no terminal:

  `$ yarn`
  `$ yarn dev`

- No insomnia, crie uma requisição (get, post, put, delete) e basta copiar as seguintes rotas:

  Método GET (listar repositórios): http://localhost:3333/repositories
  Método DELETE (deletar repositório): http://localhost:3333/repositories/dc084a6b-33c3-4720-894f-eb765d27670a
  Método POST (criar repositório): http://localhost:3333/repositories,
      		Colocar no body: 
          {
      				"url": "https://github.com/Rocketseat/umbriel",
              "title": "Umbriel",
              "techs": ["Node", "Express", "TypeScript"]
      		}

  Método POST (incrementar like): http://localhost:3333/repositories/dc084a6b-33c3-4720-894f-eb765d27670a/like,
      		Colocar no body: 
          {
      				"like": 1
      		}

  Método PUT (atualizar repositório): http://localhost:3333/repositories/dc084a6b-33c3-4720-894f-eb765d27670a,
      		Colocar no body: 
          {
      				"url": "https://github.com/Rocketseat/umbriel",
              "title": "Unform",
              "techs": ["React", "ReactNative", "TypeScript", "ContextApi"]
      		}

## Rota / Recurso
# Métodos HTTP:
- GET: Buscar uma informação do back-end
- POST: Criar uma informação no back-end
- PUT/PATH: Alterar uma informação no back-end
- DELETE: Deletar uma informação no back-end


# Tipos de parâmetros
- Query Params: Parâmetros nomeados enviados na rota após "?" (Filtros, paginação)
- Route Params: Parâmetros utilizados para identificar recursos
- Request Body: Corpo da requisição, utilizado para criar ou alterar recursos
