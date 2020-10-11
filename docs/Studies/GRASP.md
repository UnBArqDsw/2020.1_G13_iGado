
# <i>GRASP's</i>

|    Data    | Versão |         Descrição         |           Autor(es)           |
| :--------: | :----: | :-----------------------: | :---------------------------: |
| 09/10/2020 |  0.1   | Criação do Documento sobre <i>GRASP's</i> | [Caio Fernandes](https://github.com/caiovfernandes) |
| 10/10/2020 |  0.2  | Adição dos  <i>GRASP's</i> Criador e Especialista | [Caio Fernandes](https://github.com/caiovfernandes) |
| 10/10/2020 |  0.3  | Adição dos  <i>GRASP's</i> Alta Coesão e Baixo Acoplamento | [Caio Fernandes](https://github.com/caiovfernandes) |
| 10/10/2020 |  0.4  | Adição dos  <i>GRASP's</i> Controladora e Polimorfismo | [Caio Fernandes](https://github.com/caiovfernandes) |
| 10/10/2020 |  0.5  | Adição dos  <i>GRASP's</i> Invenção pura ou Fabricação Própria e Variações Protegidas | [Caio Fernandes](https://github.com/caiovfernandes) |


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


### Coesão 

<p align="justify"> &emsp;&emsp; Siginifica que suas classes estão coesas. Isso é garantido por atribuir de forma coerente a distribuição das classes utilizando padrões de projeto.

Coesão está ligada ao princípio da responsabilidade única, que foi introduzido por <i>Robert C. Martin</i> no inicio dos anos 2000 e diz que uma classe deve ter apenas uma única responsabilidade e realizá-la de maneira satisfatória, ou seja, uma classe não deve assumir responsabilidades que não são suas</p>

### Acoplamento

<p align="justify"> &emsp;&emsp;O acoplamento significa o quanto uma classe depende da outra para funcionar. E quanto maior for esta dependência entre ambas, dizemos que estas classes estão fortemente acopladas.

O forte acoplamento também nos traz muitos problemas, problemas semelhantes aos que um cenário pouco coeso nos traz. </p>

### Controladora

<p align="justify"> &emsp;&emsp;O <strong>Controlador</strong> é responsável por lidar com as solicitações dos atores. Ele é o intermediário entre o clique do usuário em “Enviar” e o back-end que faz isso acontecer. 

O Controlador sabe como interpretar as ações das interfaces de usuário e como conectar essas ações aos comportamentos em seu sistema. Este padrão permite que as interfaces de usuário sejam separadas de forma limpa dos “objetos de negócios” e tenham ambas as alterações independentementes umas das outras. Nisso está implícito que um sistema também pode suportar muitas interfaces de usuário diferentes ao mesmo tempo.

Podemos imaginar um controlador como o volante de um carro, ele conecta as intenções de um motorista às ações do veículo. Mudar o motor do carro não precisa mudar a forma como o carro é usado em alto nível. E da mesma forma, a substituição de um volante não requer que nenhum componente interno seja modificado.
A <i>Controller</i> também é um padrão importante em frameworks modernos de desenvolvimento web, formando um pilar do padrão arquitetônico <i>Model-View-Controller</i>.</p>

### Polimorfismo

<p align="justify"> &emsp;&emsp;Um conceito já conhecido e aplicado em Orientação por Objetos.

No GRASP, utiliza-se o polimorfismo ao notar que mais de uma de nossas classes tem métodos que se comportam de maneira muito parecida.

Então, cria-se um classe abstrata para ser utilizada como base. </p>

### Invenção pura ou Fabricação Própria

<p align="justify"> &emsp;&emsp;Este GRASP ocorre quando você aplica no seu projeto um serviço próprio, com um módulo novo.<br>
Ex: 

- Classes para cuidar da segurança
- Módulo de persistência no banco (DAO)
- Módulo de Autenticação de usuários
- Entre outras.. </p>


### Variações Protegidas

<p align="justify"> &emsp;&emsp;
Geralmente ocorre quando se tem Polimorfismo

A <strong>Variação Protegida (VP)</strong> é um princípio básico na motivação da maioria dos mecanismos e padrões na programação e no projeto para fornecer flexibilidade e proteção contra variações.<br>
O encapsulamento de dados, das interfaces, e o polimorfismo são mecanismos básicos para se obter a VP. As técnicas de linguagens baseada em regras, interpretadores de regra, projetos reflexivos e de metadados, máquinas virtuais, etc, são mecanismos mais avançados para se obter a VP. </p>