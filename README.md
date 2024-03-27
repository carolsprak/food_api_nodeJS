# Simulação REST API NodeJS   -  ![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=%20CONCLUÍDO&color=GREEN&style=for-the-badge)


## Começando

### 1. Crie este repositório

* Faça o download do projeto
* Abra o VSCode 
* Abra a pasta extraída do github no VsCode (no link de referência acima)
* Abra o terminal do VsCode e insira os comando para criar o repositório na pasta:

 `git init`
 
 `git add .`
 
 `git commit -m "Iniciado projeto API e NodeJS"`

 `git branch -M main`
 
 `git remote add origin url_do_repositorio` (inserir link de seu novo repositorio criado no github ex. https://github.com/seu_usuario/nome_repositorio.git)

 `git push -u origin main`


### 2. Execute o servidor na sua máquina

 
- Abrir a pasta do projeto que você baixou e acessar o terminal do VSCode 
 
- Instale o servidor Json (API Local da sua máquina)
  
   `npm install`

   
-  Execute o servidor com a base de dados

   `npm start`

## Acessando servidor local


- O servidor será executado em `http://localhost:8000`. Só abrir qualquer browser e digitar que será aberta a página inicial do API.

Você pode testar com o endpoint público: `http://localhost:8000/pizza` (método GET).

## Manipulando os dados
Com o Postment ou qualquer ferramenta de gestão de comunicação você pode alterar os dados de API, ou criar novas informações.

Para isso só utilizar os comandos abaixo.


#### Cardápio (GET)

- Obter pizzas: GET /pizza
- Obter pizza por ID: GET /pizza/{id}
- Obter massas: GET /pasta
- Obter saladas: GET /salads
- Obter sobremesas: GET /dessert
- Obter bebidas: GET /drinks
- Obter molhos: GET /sauces
- Obter acompanhamentos: GET /sides

#### Cardápio (POST)

- Obter pizzas (body): POST /pizza
- Obter massas (body): POST /pasta
- Obter saladas (body): POST /salads
- Obter sobremesas (body): POST /dessert
- Obter bebidas (body): POST /drinks
- Obter molhos (body): POST /sauces
- Obter acompanhamentos (body): POST /sides

#### Cardápio (PUT / PATCH)

- Atualizar pizza (body): PUT /pizza/{id}
- Atualizar pizza (body parcial): PATCH /pizza/{id} 
- Atualizar massa (body): PUT /massa/{id}
- Atualizar massa (body parcial): PATCH /massa/{id} 
- Atualizar salada (body): PUT /salada/{id}
- Atualizar salada (body parcial): PATCH /salada/{id} 
- Atualizar sobremesa (body): PUT /sobremesa/{id}
- Atualizar sobremesa (body parcial): PATCH /sobremesa/{id} 
- Atualizar bebida (body): PUT /bebida/{id}
- Atualizar bebida (body parcial): PATCH /bebida/{id} 
- Atualizar molho (body): PUT /molho/{id}
- Atualizar molho (body parcial): PATCH /molho/{id} 
- Atualizar acompanhamento (body): PUT /acompanhamento/{id}
- Atualizar acompanhamento (body parcial): PATCH /acompanhamento/{id} 

#### Cardápio (DELETE)

- Remover pizza: DELETE /pizza 
- Remover massa: DELETE /pasta
- Remover salada: DELETE /salads
- Remover sobremesa: DELETE /dessert
- Remover bebida: DELETE /drinks
- Remover molho: DELETE /sauces
- Remover acompanhamento: DELETE /sides


##### Exemplos de Filtros
- http://localhost:8000/pizza/1
- http://localhost:8000/pizza?spicy=true
- http://localhost:8000/pizza?name=American%20Spicy
- http://localhost:8000/pizza?spicy=true&vegetarian=false
- http://localhost:8000/pizza?spicy=true&vegetarian=true
