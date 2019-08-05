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
     5. O angular se baseia no modelo `MVC(Model, View, Controller)` e na nossa angular expression, temos {{foto.url}}, foto seria nosso `model` e quem fica no meio entre model e view, será o nosso `controller`.
     6. Boa prática criar o `controller` separado da view, criar em outra pasta.
     7. Quando criamos um módulo: `angular.module('alurapic', [])`, o array dentro dele, é o lugar onde colocamos as dependências desse módulo.
     8. Quando criamos um controller, é assim: `angular.module('alurapic').controller('FotosController', function(){});`. O primeiro parâmetro é o nome do controller, e o segundo é a função que vai conter o controller em si.
     9. A única variável global que temos que ter é o `angular`. 
          1. quando criamos o `controller`, dentro da nossa function(), a variável fica com escopo privado. E como fazemos para que tenhamos acesso a informação que está dentro do controller na view?
          2. AI QUE ENTRA O DANADO DO `$scope`
     10. A criação dos controllers, é sempre boa prática nomear com camel case.
     11. Lembrando que não existe atributos como esse no html: `ng-app`, por exemplo. O nome disso é `diretiva`. É uma espécie de liga. 
          1. por exemplo na view, index, usamos a diretiva `ng-app` para carregar/iniciar o módulo principal da aplicação. `ng-app="alurapic`
          2. a diretiva `ng-controller` serve para ligar a nossa view com nosso controller. `ng-controller="FotosController"`
      12. data binding
      13. template angular    

### Leituras externas

| assunto | links |
| --- | --- | 
| `MVC in angular world` | [leitura 1](https://scotch.io/tutorials/mvc-in-an-angular-world) |
