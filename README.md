# Desafio Dio - Criando um Jogo de Cartas do Yu-Gi-Oh! com JavaScript e CSS



Criando um Jogo de Cartas do Yu-Gi-Oh! com JavaScript e CSS

Vamos recriar um jogo do Yu-Gi-Oh utilizando as mecânicas de jogo do Jo-Ken-Po, vamos explorar conceitos avançados de organização de states com Javascript puro, estruturação de arquivos e criação de funções reaproveitáveis

**O objetivo desse projeto é desenvolver um versão do tracional jogo "Pedra, Papel e Tesoura" com inspiração na temática de Yu-Gi-Oh, utilizando apenas HTML, CSS e JavaScript.**

**Para isso, vamos utilizar o framework React.js, que é uma biblioteca JavaScript para criar interfaces de usuário.**

**Vamos começar criando um novo projeto React usando o seguinte comando:**



```plaintext
npx create-react-app jogo-de-cartas
```

**Isso irá criar uma nova pasta chamada "jogo-de-cartas", que irá conter o nosso projeto React.**

**Abra o projeto no seu editor de texto favorito e acesse o arquivo "src/App.js".**

**Nesse arquivo, vamos criar o nosso componente principal, chamado "App".**



```plaintext
import React, { Component } from "react";

class App extends Component {
  render() {
    return (
      <div>
        <h1>Jogo de Cartas</h1>
        <div>
          <button>Pedra</button>
          <button>Papel</button>
          <button>Tesoura</button>
        </div>
      </div>
    );
  }
}

export default App;
```



**Esse componente é bem simples. Ele contém um cabeçalho com o título do jogo e um bloco com três botões, cada um representando uma das opções do jogo.**

**Agora, vamos criar os componentes para cada uma das opções do jogo.**

**Vamos criar um componente chamado "Pedra" e exportá-lo como "PedraComponent".**



```plaintext
import React, { Component } from "react";

class Pedra extends Component {
  render() {
    return (
      <div>
        <img src="https://www.duelingbook.com/images/cards/S13/S13-033.jpg" alt="Pedra">
      </div>
    );
  }
}

export default PedraComponent;
```

**Esse componente é bem simples. Ele contém apenas uma imagem da carta de Pedra.**

**Vamos criar os componentes para as outras opções do jogo da mesma forma.**

**Agora, vamos voltar para o componente "App" e modificá-lo para que ele exiba os componentes para as três opções do jogo.**



```plaintext
import React, { Component } from "react";

import PedraComponent from "./PedraComponent";
import PapelComponent from "./PapelComponent";
import TesouraComponent from "./TesouraComponent";

class App extends Component {
  render() {
    return (
      <div>
        <h1>Jogo de Cartas</h1>
        <div>
          <PedraComponent />
          <PapelComponent />
          <TesouraComponent />
        </div>
      </div>
    );
  }
}

export default App;
```



**Agora, o nosso componente "App" está exibindo os componentes para as três opções do jogo.**

**Podemos ver o resultado clicando no link da pasta "build".**

**O jogo está funcional, mas ainda está um pouco feio.**

**Vamos deixar ele mais bonito aplicando alguns estilos CSS.**

**Vamos criar um arquivo chamado "App.css" e colocar nele o seguinte código:**



```plaintext
body {
  margin: 0;
  padding: 0;
  font-family: sans-serif;
}

h1 {
  text-align: center;
  margin: 0;
  padding: 20px;
  font-size: 24px;
}

.carta {
  width: 150px;
  height: 200px;
  margin: 10px;
  display: inline-block;
}
```



**Esse código CSS irá aplicar alguns estilos básicos ao nosso componente "App".**

**Podemos ver o resultado clicando no link da pasta "build".**

**O nosso jogo está ficando mais bonito!**

**Agora, vamos adicionar um pouco de lógica ao nosso jogo.**

**Vamos criar um método chamado "escolherCarta" que irá retornar uma carta aleatória.**



```
import React, { Component } from "react";

import PedraComponent from "./PedraComponent";
import PapelComponent from "./PapelComponent";
import TesouraComponent from "./TesouraComponent";

class App extends Component
```
