
# <i>GRASP's</i>

|    Data    | Versão |         Descrição         |           Autor(es)           |
| :--------: | :----: | :-----------------------: | :---------------------------: |
| 09/10/2020 |  0.1   | Criação do Documento sobre <i>GRASP's</i> | [Caio Fernandes](https://github.com/caiovfernandes) |
| 10/10/2020 |  0.2  | Adição do  <i>GRASP</i> Criador e Especialista | [Caio Fernandes](https://github.com/caiovfernandes) |


<p align="justify"> &emsp;&emsp; <i>Design Patterns</i> são ferramentas incrivelmente importantes para desenvolvedores de software. Acima de resolver problemas comuns, eles fornecem às pessoas um vernáculo padrão para se comunicarem e oferecem abstrações conceituais valiosas em um amplo conjunto de circunstâncias.
GRASP significa General Responsability Assignment Software Patterns. Esses padrões, como o nome sugere, visam principalmente responder à pergunta: "Quem faz o quê?"</p>

<p align="justify"> &emsp;&emsp; GRASP é um conjunto de 9 padrões de software de atribuição de responsabilidade geral. São eles:</p>

- Criador
- Especialista
- Alta Coesão
- Baixo Acoplamento
- Controladora
- Polimorfismo
- Invenção pura ou Fabricação Própria
- Indireção
- Variações Protegidas


### Criador
<p align="justify"> &emsp;&emsp; O Criador assume a responsabilidade de criar outros objetos. Esse padrão é provavelmente o mais fácil de entender conceitualmente. Existem vários motivos pelos quais uma classe pode assumir a responsabilidade de criar outra.

O Criador pode ter informações sobre como criar o referido objeto, ou pode ser a classe que usa o objeto mais de perto. Essas decisões serão amplamente estabelecidas no design inicial do sistema, e outros documentos, como diagramas UML, guiarão e informarão o padrão do Criador.
O GRASP Criador permite que muitas outras práticas recomendadas se encaixem, como injeção de dependência e baixo acoplamento. O Padrão do Criador pode ser usado para reforçar o design lógico de um sistema.

Em geral, uma classe `B` deve ser responsável por criar instâncias de classe `A` se uma, ou preferencialmente mais, das seguintes afirmações se aplicam:

- Instâncias de `B` contêm ou agregam instâncias de `A`;
- Instâncias de `B` gravam instâncias de `A`;
- Instâncias de `B` utilizam de perto instâncias de `A`;
- Instâncias de `B` têm as informações de iniciação das instâncias de `A` e passam isso na criação.</p>


### Especialista

<p align="justify"> &emsp;&emsp; A medida que os sistemas crescem, podemos descobrir que estamos colocando muita lógica em nossos controladores. Isso resulta no que chamamos de “controladores inchados”. Controladores inchados implicam em um acoplamento forte em nosso sistema, o que é ruim.<br>
O GRASP Especialista resolve isso encapsulando informações sobre uma tarefa em uma classe distinta. Isso pode parecer um pouco abstrato, mas vamos trabalhar com um exemplo simples:<br>
A autenticação do usuário é um problema comum. Podemos ter um usuário que está logando para ter seu nome de usuário e senha validados no sistema. Com apenas um controlador, isso pode ter a seguinte aparência:<br><br>
Login do usuário → Controlador → Banco de dados<br><br>
Esta transação requer muito trabalho por parte do Controlador. A autenticação pode envolver hashing, pesquisas de banco de dados e talvez outras tarefas específicas do aplicativo. Portanto, apresentamos  um especialista: <strong>Módulo de autenticação</strong>.<br>

Este módulo sabe exatamente como autenticar um usuário, e o Controlador precisa apenas delegar a solicitação de autenticação a este módulo para saber que a autenticação será tratada corretamente.<br><br>
Solicitação de login → Controlador → Módulo de autenticação → Banco de dados<br><br>
Dessa forma, o padrão <strong>GRASP Especialista</strong> é muito parecido com um especialista no mundo real. Quando desejamos construir uma casa, podemos contar com a ajuda de um arquiteto. É possível para uma pessoa projetar sua própria casa (e muitas pessoas fazem), mas na maioria das vezes preferiríamos terceirizar essa tarefa. As pessoas já têm o suficiente para administrar ao construir uma casa, e um arquiteto certamente está mais bem equipado para projetar casas.</p>