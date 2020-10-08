# Dojo de Flutter
|    Data    | Versão |                Descrição                |                     Autor(es)                     |
| :--------: | :----: | :-------------------------------------: | :-------------------------------------------: |
| 06/10/2020 |  0.1   | Criação dos Diagramas iniciais da estrutura do front | [Iuri Severo](https://github.com/iurisevero) e [João Guedes](https://github.com/sudjoao) |
| 08/10/2020 |  0.2   | Cronograma do Dojo | [Iuri Severo](https://github.com/iurisevero) e [João Guedes](https://github.com/sudjoao) |
| 08/10/2020 |  0.3   | Detalhamento do Dojo | [Iuri Severo](https://github.com/iurisevero) e [João Guedes](https://github.com/sudjoao) |
| 08/10/2020 | 0.4 | Adição dos tópicos Stateless e Stateful Widgets e Arquivo de Constantes | [Iuri Severo](https://github.com/iurisevero) e [João Guedes](https://github.com/sudjoao) |
| 08/10/2020 |  0.5 | Adição das árvores de login e registro | [Iuri Severo](https://github.com/iurisevero) e [João Guedes](https://github.com/sudjoao) |

## Cronograma de Conteúdos

* O que é Flutter? 
* A estrutura de Flutter; 
* O que são widgtes? 
    * Scaffold; 
    * Container;
    * Row;
    * Column;
    * Image.
* Pubspec.yaml pra que serve?
    * Utilizar para pegar os ícones;
    * Importar alguma imagem na prática;
* Statefull e Stateless;
    * Componentização;
        * Orientação a objetos;
* Fazendo outras telas;
* Navegação entre telas;
    * Navigator;
    * Routes;
* Arquivo de constantes.

## Conteúdos
### O que é Flutter?
["Flutter is Google’s UI toolkit for building beautiful, natively compiled applications for mobile, web, and desktop from a single codebase."](https://flutter.dev/)

Flutter é um conjunto de ferramentas que facilitam o desenvolvimento de interfaces de tamanhos variados e para todos tipos de aparelho. De modo simplificado, o Flutter "pede" para o aparelho uma tela em branco e adiciona _widgets_ pré-montados nela, o que faz funcionar para Android e IOs, independente do tamanho da tela.

### A estrutura do Flutter
Tudo dentro de um aplicativo em Flutter é considerado um _widget_, é durante a criação das telas o programador constrói blocos de _widgets_, adicionando-os um acima do outro, como lego. No fim, o desenvolvedor constrói uma árvore de _widgets_, como a do exemplo abaixo:

<img src="docs/Assets/Img/Studies/DojoFlutter/SplashScreenTree.png" alt="Splash Screen Tree" height=500>

### O que são _widgets_?
["Widgets describe what their view should look like given their current configuration and state. When a widget’s state changes, the widget rebuilds its description, which the framework diffs against the previous description in order to determine the minimal changes needed in the underlying render tree to transition from one state to the next."](https://flutter.dev/docs/development/ui/widgets-intro)

Basicamente, Widgets são estruturas que se constroem a partir de um estado descrito pela aplicação. Quando esse estado muda, a estrutura se reconstroe para ficar de acordo com o estado atual. Alguns _widgets_ básicos são:
* Scaffold; 
* Container;
* Row;
* Column;
* Image.

### Pubspec.yaml pra que serve?
É um arquivo que guarda o metadata dos pacotes utilizados pela aplicação, assim como suas dependências. Nele é possível realizar diversas alterações, como o nome do aplicativo, seu ícone e a adição de Assets.

### Stateful e Stateless
Em flutter podemos separar os widgets em widgets que podem mudar de estado(Stateful) e widgets que não mudam de estado(Stateless). 

Um widget stateless é um widget estático, que vai sempre continuar do mesmo jeito independente da interação que o usuário faz, um exemplo disso pode ser um texto que aparece na tela.


Dizer que um widget é stateful significa que ele tem a capacidade de mudar de estado a partir de alguma interação externa, como um clique em um botão etc, ou seja a principal característica de um widget stateful é ele ser dinâmico.

As mudanças de estado ocorridas em um stateful widget são causadas a partir da utilização da função setState() que pode ser utilizada , por exemplo, para uma aplicação de uma calculadora, onde a pessoa vai clicando nos números e operações e os mesmos vão aparecendo na tela de forma que quase instantânea.  

Mais informações sobre em: <https://flutter.dev/docs/development/ui/interactive>


### Fazendo outras telas
Nesse dojo serão elaboradas duas telas, a de Login e a de Registro. Elas seguirão as árvores abaixo:

<img src="docs/Assets/Img/Studies/DojoFlutter/LoginScreenTree.png" alt="Login Screen Tree" height=500>
<br /><br />
<img src="docs/Assets/Img/Studies/DojoFlutter/RegisterScreenTree.png" alt="Register Screen Tree" height=500>

### Navegação entre telas
A navegação entre telas do Flutter é feita a partir de um _widget_ que gerencia _widgets_ "filhos" em um comportamento de pilha. Esse _widget_ é o **Navigator**, enquanto seus "filhos" são as **Rotas**. 

Mais informações sobre o sistema de navegação do Flutter estão disponível em <https://flutter.dev/docs/development/ui/navigation/>

### Arquivo de constantes

Para facilitar a utilização de alguns estilizações que ocorrem em várias partes do aplicativo e evitar repetição de código o grupo viu a necessidade de ter um arquivo onde guardarão todas essas constantes de estilo para quando forem utilizar simplesmente importarem.

A ideia deste arquivo foi tirada do curso [The Complete 2020 Flutter Development Bootcamp with Dart](https://www.udemy.com/course/flutter-bootcamp-with-dart/?utm_source=adwords&utm_medium=udemyads&utm_campaign=LongTail_la.EN_cc.ROW&utm_content=deal4584&utm_term=_._ag_77879424134_._ad_437497333833_._kw__._de_c_._dm__._pl__._ti_dsa-1007766171312_._li_9074205_._pd__._&matchtype=b&gclid=Cj0KCQjw8fr7BRDSARIsAK0Qqr5Idg1WmuFhvV1o3gNf_u_WEedhlAQ4TCG1G-2MnomMMxuuDl1LMhAaAmRvEALw_wcB) da Dr. Angela Yu.

## Referências

* https://flutter.dev/ , acessado em setembro de 2020;
* https://flutter.dev/docs, acessado em setembro de 2020;
* https://dart.dev/tools/pub/pubspec, acessado em setembro de 2020;
* YU, Angela. Complete Flutter App Development Bootcamp with Dart. Acessado em setembro de 2020.
