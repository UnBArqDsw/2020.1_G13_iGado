# GoFs Estruturais

|    Data    | Versão |         Descrição         |           Autor(es)           |
| :--------: | :----: | :-----------------------: | :---------------------------: |
| 09/10/2020 |  0.1   | Criação do Documento sobre GoFs Estruturais | [Lucas Fellipe](https://github.com/lucasfcm9) |
| 09/10/2020 |  0.4   | Adição do Padrão Adapter e do Padrão Composite | [Lucas Fellipe](https://github.com/lucasfcm9) |
| 09/10/2020 |  0.6   | Adição do Padrão Decorator | [Lucas Fellipe](https://github.com/lucasfcm9) |

<p align="justify"> &emsp;&emsp; Os GoFs Estruturais explicam como montar objetos e classes em estruturas maiores, porém mantendo essas estruturas flexíveis e eficientes. Eles mexem na estrutura dos modelos presentes e em como esses modelos estão interagindo. São padrões que atuam de forma significante nas correlações entre as classes e nas relações de depedência. Os Padrões Estruturais se preocupam com as interações entre os objetos. Dessa forma, os Padrões Estruturais têm como objetivo diminuir essa dependência entre os objetos. Serão apresentados os seguintes Padrões Estruturais: Adapter, Composite, FlyWeight, Decorator, Proxy, Bridge e o Facade. </p>

## Adapter
<p align="justify"> &emsp;&emsp; O Adapter permite que um objeto seja substituído por outro e, apesar de realizarem a mesma tarefa, possuem interfaces diferentes. Ele serve como um adaptador, ou seja, É um objeto especial que converte a interface principal de um objeto para que outro objeto possa entendê-lo. Você pode utilizar o Adapter quando você quer usar uma classe existente, porém a sua interface não é compatível com o restante do código. O Adapter ajuda que objetos com diferentes interfaces colaborem entre si, por exemplo: </p>

- O Adapter obtém uma interface, compatível com um dos objetos existentes;
- Usando essa interface, o objeto existente pode chamar os métodos do Adapter com segurança;
- Ao receber a chamada, o Adapter passa o pedido para o segundo objeto, mas em um formato e ordem que o segundo objeto espera.

<img src="https://user-images.githubusercontent.com/40740008/95642285-f276e500-0a7d-11eb-92f9-914cb8a2ebb8.jpg" width="500px"/> <br>

Este é um exemplo do padrão Adapter, onde adaptamos a Entrada PS2 para a Entrada USB.

## Composite
<p align="justify"> &emsp;&emsp; O Composite é um padrão de projeto estrutural que tem como objetivo agrupar objetos que fazem parte de uma relação parte-todo de forma a tratá-los sem distinção. Uma interface, ou até mesmo uma classe abstrata, é implementada por diversas outras classes. Ele permite com que você componha objetos em estruturas de árvores e então trabalhe com essas estruturas como se elas fossem objetos individuais. Você pode utilizar o padrão Composite quando você tem que implementar uma estruturas de objetos tipo árvore.</p>

<img src="https://user-images.githubusercontent.com/40740008/95642804-48995780-0a81-11eb-82f3-7c57304f23ed.png" width="600px"> <br>
A estrutura do Composite é formada por uma <i>Interface</i>, por <i>leafs</i> e pela classe Composite.


<!-- Interface - Trecho
     Leafs - Sub-trechos
     Composite - Caminho todo

     Interface - Comida (Fast Food)
     Leaf - Carne, queijo, tomate, etc.
     Composite - Hambúrguer (Leaf1 + Leaf2 + Leaf3...(Carne, queijo, tomate, etc.)). Ele é formado por várias leafs, ou sera, várias comidas
-->

## Decorator
<p align="justify"> &emsp;&emsp; O Decorator é um padrão de projeto estrutural que permite adicionar responsabilidades a um objeto de maneira dinâmica, criando algo similar a uma extensão do objeto. Ele permite, a partir de uma base, anexar novos comportamentos aos objetos. </p>

<img src="https://user-images.githubusercontent.com/40740008/95643225-52708a00-0a84-11eb-9470-6c6456df50cd.png" width="600px"/> <br>

Pode-se ver que há um Decorator Base, que servirá como um ponte entre o Client e os Decorators que realmente irão alterar o comportamento do objeto concreto.

### Exemplo
<img src="https://user-images.githubusercontent.com/40740008/95643304-cad74b00-0a84-11eb-8dfc-d106ac0b4770.png" width="500px">









