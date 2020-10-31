# Nome do projeto

(Re)pense

## Alunos integrantes da equipe

* Marcos Lucas De Moura Lacerda
* Naiara Marques Santos
* Maycon Gomes Silva
* Caio Henrique Lucas Gonçalves Furbino
* Daniel Schlickmann Bastos
* Giovani Andrade Maletta
* Daniel Arthur Neves Da Silva

## Professores responsáveis

* Simone Alves Nogueira
* Roberto Felipe Dias Ferreira Da Roch

## Deploy

A pasta `Codigo` contém, obviamente, o código. Temos que fazer push para o Heroku somente dessa pasta, e não deste repositório inteiro. Dado isso, teremos duas origens no git, a `origin` (essa do Github) e a do Heroku, `heroku`.

Para adicionar o remoto do Heroku, execute o seguinte comando:

- Caso você utilize https: `git remote add heroku https://git.heroku.com/tiw-repense.git`
- Caso você utilize ssh: `git remote add heroku git@heroku.com:tiw-repense.git`

Você precisa pedir para o @danielSbastos para ter acesso de escrita no Heroku.

Agora, para dar push, é necessário rodar o seguinte comando do root do projeto (não é um push comum pois estamos dando push somente de uma pasta).

- `git subtree push --prefix Codigo heroku main`

A seguinte URL é a do projeto, onde será possível ver as novas alterações refletidas: https://tiw-repense.herokuapp.com/
