# <i>GoFs Estruturais</i>

|    Data    | Versão |         Descrição         |           Autor(es)           |
| :--------: | :----: | :-----------------------: | :---------------------------: |
| 09/10/2020 |  0.1   | Criação do Documento sobre <i>GoFs Estruturais</i> | [Lucas Fellipe](https://github.com/lucasfcm9) |
| 09/10/2020 |  0.2   | Adição do Padrão <i>Adapter</i> e do Padrão <i>Composite</i> | [Lucas Fellipe](https://github.com/lucasfcm9) |
| 09/10/2020 |  0.3   | Adição do Padrão <i>Decorator</i> | [Lucas Fellipe](https://github.com/lucasfcm9) |
| 10/10/2020 |  0.4   | Adição do Padrão <i>Bridge</i>, <i>Facade</i>, <i>Proxy</i> e <i>FlyWeight</i> | [Lucas Fellipe](https://github.com/lucasfcm9) |
| 10/10/2020 |  1.0   | Revisão do documento | [Iuri Severo](https://github.com/iurisevero) |
| 26/10/2020 | 1.1 | Adição do vídeo de apresentação dos padrões para o grupo | [João Pedro Guedes](https://github.com/sudjoao)|

## Introdução
<p align="justify"> &emsp;&emsp; Os <i>GoFs Estruturais</i> explicam como montar objetos e classes em estruturas maiores, porém mantendo essas estruturas flexíveis e eficientes. Eles mexem na estrutura dos modelos presentes e em como esses modelos estão interagindo. São padrões que atuam de forma significante nas correlações entre as classes e nas relações de depedência. <br /> &emsp;&emsp;
Os Padrões Estruturais se preocupam com as interações entre os objetos. Dessa forma, os Padrões Estruturais têm como objetivo diminuir essa dependência entre os objetos. Serão apresentados os seguintes Padrões Estruturais: <i>Adapter</i>, <i>Composite</i>, <i>FlyWeight</i>, <i>Decorator</i>, <i>Proxy</i>, <i>Bridge</i> e o <i>Facade</i>. </p>

<a href="https://www.youtube.com/watch?v=wKXm9As171k&feature=youtu.be">Vídeo de Apresentação dos Padrões para o grupo</a>

## Adapter
<p align="justify"> &emsp;&emsp; O <i>Adapter</i> permite que um objeto seja substituído por outro e, apesar de realizarem a mesma tarefa, possuem interfaces diferentes. Ele serve como um adaptador, ou seja, é um objeto especial que converte a interface principal de um objeto para que outro objeto possa entendê-lo. Você pode utilizar o <i>Adapter</i> quando você quer usar uma classe existente, porém a sua interface não é compatível com o restante do código. O <i>Adapter</i> ajuda que objetos com diferentes interfaces colaborem entre si, por exemplo: </p>

- O <i>Adapter</i> obtém uma interface, compatível com um dos objetos existentes;
- Usando essa interface, o objeto existente pode chamar os métodos do <i>Adapter</i> com segurança;
- Ao receber a chamada, o <i>Adapter</i> passa o pedido para o segundo objeto, mas em um formato e ordem que o segundo objeto espera.

### Estrutura

<img src="https://user-images.githubusercontent.com/40740008/95658637-563af580-0af2-11eb-8822-b5515342fc72.png" width="600px"/>

### Exemplo

<img src="https://user-images.githubusercontent.com/40740008/95642285-f276e500-0a7d-11eb-92f9-914cb8a2ebb8.jpg" width="500px"/> <br>

Este é um exemplo do padrão <i>Adapter</i>, onde adaptamos a Entrada PS2 para a Entrada USB.

## Composite
<p align="justify"> &emsp;&emsp; O <i>Composite</i> é um padrão de projeto estrutural que tem como objetivo agrupar objetos que fazem parte de uma relação parte-todo de forma a tratá-los sem distinção. Uma interface, ou até mesmo uma classe abstrata, é implementada por diversas outras classes. Ele permite com que você componha objetos em estruturas de árvores e então trabalhe com essas estruturas como se elas fossem objetos individuais. Você pode utilizar o padrão <i>Composite</i> quando você tem que implementar uma estruturas de objetos tipo árvore.</p>

### Estrutura

<img src="https://user-images.githubusercontent.com/40740008/95658693-b467d880-0af2-11eb-832f-c2a6c55373f5.png" width="600px"> <br>
A estrutura do <i>Composite</i> é formada por uma <i>Interface</i>, por <i>leafs</i> e pela classe <i>Composite</i>.


<!-- Interface - Trecho
     Leafs - Sub-trechos
     <i>Composite</i> - Caminho todo

     Interface - Comida (Fast Food)
     Leaf - Carne, queijo, tomate, etc.
     <i>Composite</i> - Hambúrguer (Leaf1 + Leaf2 + Leaf3...(Carne, queijo, tomate, etc.)). Ele é formado por várias leafs, ou sera, várias comidas
-->

## Decorator
<p align="justify"> &emsp;&emsp; O <i>Decorator</i> é um padrão de projeto estrutural que permite adicionar responsabilidades a um objeto de maneira dinâmica, criando algo similar a uma extensão do objeto. Ele permite, a partir de uma base, anexar novos comportamentos aos objetos. </p>

### Estrutura

<img src="https://user-images.githubusercontent.com/40740008/95658753-19bbc980-0af3-11eb-88ed-4f396de3a49c.png" width="600px"/> <br>

Pode-se ver que há um <i>Decorator</i> Base, que servirá como um ponte entre o Client e os <i>Decorator</i>s que realmente irão alterar o comportamento do objeto concreto.

### Exemplo
<img src="https://user-images.githubusercontent.com/40740008/95658783-5a1b4780-0af3-11eb-841e-4eafd430aa9a.png" width="500px">

## Bridge
<p align="justify"> &emsp;&emsp; O <i>Bridge</i> é um padrão de projeto que permite que você divida uma classa grande ou um conjunto de classes intimamente ligadas em duas hierarquias separadas que podem ser desenvolvidas separadamente, sem uma depender da outra. De forma simplificada, esse padrão permite a divisão de uma classe em implementações menores.</p>

### Estrutura

<img src="https://user-images.githubusercontent.com/40740008/95658553-ae252c80-0af1-11eb-8156-f9b64b0b355e.png" width="600px"/>

### Exemplo
<img src="https://user-images.githubusercontent.com/40740008/95659021-d2363d00-0af4-11eb-8aa7-17a927538c2d.png" width="500px"/>

<!-- A classe de controle remoto base declara um campo de referência que liga ela com um objeto de dispositivo. Todos os controles trabalham com dispositivos através da interface geral de dispositivo, que permite que o mesmo controle suporte múltiplos tipos de dispositivo.</p>

Você pode desenvolver as classes de controle remoto independentemente das classes de dispositivo. -->

## Facade
<p align="justify"> &emsp;&emsp; O <i>Facade</i> é um padrão de projeto estrutural que fornece uma interface simplificada para uma biblioteca, um framework ou qualquer conjunto complexo de classes.</p>

### Estrutura
<img src="https://user-images.githubusercontent.com/40740008/95660103-fcd7c400-0afb-11eb-84d7-34f4c95b38c2.png" width="600px"/>

### Exemplo
<img src="https://user-images.githubusercontent.com/40740008/95660157-53450280-0afc-11eb-8251-41378fbbecc3.png" width="500px"/>

<!-- Pensa em uma biblioteca disponível no C++, por exemplo, pensa na biblioteca string.h. Ela possui diversas funções disponíveis, ela é um <i>facade</i>. Pensa também no Flask, que é um Framework usado para desenvolvimento web, por exemplo. -->

## Proxy
<p align="justify"> &emsp;&emsp; O <i>Proxy</i> é um padrão de projeto estrutural que permite que você forneça um substituto para outro objeto. Um <i>proxy</i> controla o acesso ao objeto original, permitindo que você faça algo antes ou depois do pedido chegar ao objeto original.</p>

### Estrutura
<img src="https://user-images.githubusercontent.com/40740008/95660406-11b55700-0afe-11eb-9fda-17e8572c504d.png" width="600px"/>

### Exemplo
<img src="https://user-images.githubusercontent.com/40740008/95660433-46291300-0afe-11eb-8b9c-6e7939937ff9.png" width="500px"/>

<!-- Um cartão de crédito é um <i>proxy</i> para uma conta bancária, que é um <i>proxy</i> para uma porção de dinheiro. Ambos implementam a mesma interface porque não há necessidade de carregar uma porção de dinheiro por aí. Um cliente se sente bem porque não precisa ficar carregando montanhas de dinheiro por aí. Um dono de loja também fica feliz uma vez que a renda da transação é adicionada eletronicamente para sua conta sem o risco de perdê-la no depósito ou de ser roubado quando estiver indo ao banco. -->

## Flyweight
<p align="justify"> &emsp;&emsp; O método do <i>FlyWeight</i> surgiu para solucionar o problema de gerenciamento de memória em programas que consomem bastante RAM. Basicamente, ele é uma otimização.</p>

### Estrutura
<img src="https://user-images.githubusercontent.com/40740008/95660658-aff5ec80-0aff-11eb-9661-e325e481cc40.png" width="600px"/>

<p align="justify"> &emsp;&emsp; A classe <i>FlyWeight</i> fica responsável por guardar as instâncias dos objetos que antes eram repetidas. Dessa forma, o consumo de memória reduz drasticamente e a classe <i>FlyWeight</i> compartilha, via métodos, para as demais partes do sistema.</p>


## Referências
* REFACTORING GURU: Padrões de projeto estruturais. 2014-2020. Disponível em: <https://refactoring.guru/pt-br/design-patterns/structural-patterns>. Acesso em: 09 out. 2020.
* DEVMEDIA. Entendendo os conceitos dos Padrões de Projetos em Java. Disponível em: <https://www.devmedia.com.br/entendendo-os-conceitos-dos-padroes-de-projetos-em-java/29083>. Acesso em: 09 out. 2020.
* DEVMEDIA. Design Patterns: Padrões “GoF”. Disponível em: <https://www.devmedia.com.br/design-patterns-padroes-gof/16781>. Acesso em: 09 out. 2020.
* SERRANO, Milene. Arquitetura e Desenho de Software AULA - <i>GoFs Estruturais</i>. Acesso em: 09 out. 2020.