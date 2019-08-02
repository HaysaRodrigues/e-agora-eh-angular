# E agora? é angular
Organizar estudos sobre angular 1.v 

### Ambiente 
1. Setup do [angular v1](https://angularjs.org/)

### Fundação 
1. Angular organiza a aplicação em módulos
     1. existe um módulo fundamental para criação da aplicação, que é chamado quando iniciamos a aplicação. Normalmente, chamamos de `main.js`
     2. quando estamos trabalhando no contexto do `angular`, chamamos de `view` tudo o que é `página`. 
     3. `angular expression` é o nome que damos para "lacunas" que criamos dentro da nossa view(elas ficam dentro das chaves): 
     `<img src={{foto.url}}>`
     4. Importante lembrar que por padrão, se a `angular expression` não estiver sendo carregada, não vamos identificar o erro, pois por padrão o angular ignora e deixa em branco.
     4. O angular se baseia no modelo `MVC(Model, View, Controller)` e na nossa angular expression, temos {{foto.url}}, foto seria nosso `model` e quem fica no meio entre model e view, seria o nosso `controller`.
    