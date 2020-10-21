# GoFs Comportamentais

|    Data    | Versão |         Descrição         |           Autor(es)           |
| :--------: | :----: | :-----------------------: | :---------------------------: |
| 10/10/2020 | 0.1 | Criação do Documento de GoFs Comportamentais |[João Pedro José](https://github.com/sudjoao) |
| 10/10/2020 | 0.2 | Criação da Introdução do Documento |[João Pedro José](https://github.com/sudjoao)|
| 10/10/2020 | 0.3 | Adição dos padrões comportamentais |[João Pedro José](https://github.com/sudjoao)|
| 10/10/2020 | 0.4 | Adição das padrões Referências |[João Pedro José](https://github.com/sudjoao)|
| 10/10/2020 | 1.0 | Revisão do documento |[Iuri Severo](https://github.com/iurisevero)|

## Introdução

<p align="justify"> &emsp;&emsp; Segundo o livro <i>Design Patterns: Elements of Reusable Object-Oriented Software</i>,  os padrões comportamentais estão preocupados com algoritmos e a atribuição de responsabilidades entre objetos. Os padrões comportamentais descrevem não apenas os padrões de objetos ou classes, mas também os padrões de comunicação entre eles. Estes padrões caracterizam o fluxo de controle complexo que é difícil de seguir em tempo de execução. Eles mudam seu foco do fluxo de controle para permitir que você se concentre apenas em objetos do caminho que estão interconectados. <br />&emsp;&emsp;
Existem vários padrões que são abordados na parte comportamental, cada um preocupado com uma coisa e que tem um objetivo específico, como será específicado logo abaixo.</p>

## Padrões Comportamentais

### Command
Padrão responsável pela chamada de um determinado componente, além disso ele é responsável por controlar suas requisições, muito ligado a questão de encapsulamento.

<img src='docs/Assets/Img/Studies/GoFs/Command.png'>

### Chain of Responsibility
Tem como objetivo evitar a dependência entre um objeto receptor e um objeto solicitante. Mantém guardado um ponteiro com o seu sucessor.

<img src='docs/Assets/Img/Studies/GoFs/ChainOfResponsibility.png'>

### Iterator
Fornece uma maneira de acessar elementos de uma agregação de objetos sequencialmente.

<img src='docs/Assets/Img/Studies/GoFs/Iterator.png'>

### Mediator 
Responsável por diminuir a ligação entre vários objetos, faz isso a partir da criação de um mediador que ficará responsável por fazer todas essa comunicação.

<img src='docs/Assets/Img/Studies/GoFs/Mediator.png'>

### Memento
Armazena um estado interno de um objeto em um determinado momento para que depois seja possível você voltar para aquele estado anterior do objeto.

<img src='docs/Assets/Img/Studies/GoFs/Memento.png'>

### Observer
Definição de um mecanismo eficiente, normalmente utilizando uma dependência de *um para muitos*, para reagir às alterações realizadas em determinados objetos.

<img src='docs/Assets/Img/Studies/GoFs/Observer.png'>

### State
Permite um objeto alterar seu comportamento quando um estado interno é alterado.

<img src='docs/Assets/Img/Studies/GoFs/State.png'>

### Strategy
Define uma família de algoritmos que têm um mesmo objetivo, mas dependendo do contexto inserido será selecionado o algortimo que faz mais sentido para resolver aquele problema.

<img src='docs/Assets/Img/Studies/GoFs/Strategy.png' height=350>

### Template Method
Define uma ordem lógica, ou esqueleto, de ações que devem ser realizadas no sistema, a ordem sempre continuará a mesma mas os ações realizadas podem ser realizadas de maneira diferente dependendo da sub-classe que a está executando.

<img src='docs/Assets/Img/Studies/GoFs/TemplateMethod.png' height=350>

### Visitor
Representa uma operação a ser executada em elementos de um objeto. O padrão visitor permite a definição de uma nova operação sem fazer alterações nos elementos das classes onde ele opera.

<img src='docs/Assets/Img/Studies/GoFs/Visitor.png'>


## Referências
* GAMMA, Erich; HELM, Richard; JOHNSON, Ralph; VLISSIDES, John. Design Patterns: Elements of Reusable Object-Oriented Software Addison-Wesley Professional (1994). Acesso em: 10 out. 2020.
* CARR, Richard. Gang of Four Design Patterns. Disponível em: http://www.blackwasp.co.uk/gofpatterns.aspx. Acesso em: 10 out. 2020.
* DEVMEDIA. Design Patterns: Padrões "GoF". Disponível em: https://www.devmedia.com.br/design-patterns-padroes-gof/16781. Acesso em: 10 out. 2020.
* SERRANO, Milene. Arquitetura e Desenho de Software AULA - GoFs Comportamentais. Acesso em: 10 out. 2020.


