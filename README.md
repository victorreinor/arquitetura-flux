# Arquitetura Flux
Estudos e boas práticas da arquitetura flux (redux, redux-saga, reactotron)


### Redux Saga
---
Utilizamos o redux-saga sempre que precisar fazer qual quer tipo de verificação, qual quer tipo de side effects na hora de manipular um dado dentro de redux.

Então sempre que quisermos fazer uma verificação asincrona ou tipo de side effect (chamadas em api, chamadas em banco, async storage) ou qualquer outra coisa asincrona antes de uma informação ser alterada no reducer nos utilizamos o redux-saga
