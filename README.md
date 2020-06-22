# Arquitetura Flux
Estudos e boas práticas da arquitetura flux (redux, redux-saga, reactotron)


### Redux
---
É uma biblioteca que implementa arquitetura flux (pode ser usada com angular, react, javascript puro ou em qualquer outra biblioteca front-end).

Arquitetura flux é uma forma de comunicação entre varios elementos de tela.
Serve para controlar estados globais da nossa aplicação.

**Quando utilizar ?**
- Quando o estado tem mais de um dono;
- Quando o estado é manipulado por mais componentes. Ex: carrinho de compras de um e-commerce;
- Quando as ações do usuário causam efeitos colaterais nos dados;
	- Ex: Quando adicionar um produto no carrinho, deveria disparar uma mensagem em algum lugar da tela ou mudar algum contador na tela em outro componente

O Redux começa fazer sentido quando precisamos de dados que são manipulados por multiplos componentes na aplicação e esses dados precisam estar dispostos nesses componentes, então para isso utilizamos um estado global, é como se fosse um componente que tem um estado global e todo mundo pode utilizar e manipular esses dados.

*Estados Globais: São estados que não tem um dono específico, quando varios componentes utilizam o mesmo estado e manipulam o mesmo estado.*

### Redux Saga (middleware)
---
redux-saga é uma biblioteca que foca em fazer os efeitos colaterais (ex: chamadas assíncronas para buscar dados em uma API, transformações impuras como acessar o cache do navegador, etc) em aplicações React/Redux serem mais fáceis e simples de se criar e manter.

Utilizamos o redux-saga sempre que precisar fazer qual quer tipo de verificação, qual quer tipo de side effects na hora de manipular um dado dentro de redux.
Então sempre que quisermos fazer uma verificação asincrona ou tipo de side effect (chamadas em api, chamadas em banco, async storage) ou qualquer outra coisa asincrona antes de uma informação ser alterada no reducer nos utilizamos o redux-saga

## Passo-a-passo para rodar a aplicação

### `https://github.com/victorreinor/arquitetura-flux`
Clona o repositorio do projeto;

### `cd arquitetura-flux`
Entra dentro da pasta do projeto;

### `yarn global add json-server`
Instala dependencia para criar um API Rest falsa;

### `yarn install`
Baixa as dependencias que são utilizadas no projeto;

### `json-server server.json -p 3333`
Este comando ira iniciar o servidor json na porta 3333;

### `yarn start`
Para iniciar a aplicação em desenvolvimento;


### `code .`
Para abrir o terminal;

