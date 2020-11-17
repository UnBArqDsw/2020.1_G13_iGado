# **Documento de Arquitetura de Software**

## **Histórico de Revisão**

| **Data** | **Versão** | **Descrição** | **Autor(es)** |
| --- | --- | --- | --- |
| 04/11/2020 | 0.1 | Criação do Documento | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 04/11/2020 | 0.2 | Tópico 1 - Introdução | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 04/11/2020 | 0.3 | Tópico 2 - Representação Arquitetural | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 04/11/2020 | 0.4 | Tópico 3 – Metas e Restrições de Arquitetura | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 05/11/2020 | 0.5.1 | Tópico 4 – Casos de Uso - Diagramas e Fluxos Básicos | [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) |
| 05/11/2020 | 0.5.2 | Tópico 4 – Casos de Uso - Descrição dos Casos de Uso e Fluxos Alternativos | [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) |
| 09/11/2020 | 0.6 | Tópico 5 – Lógico:  Diagrama de Pacotes | [Caio Fernandes](https://github.com/caiovfernandes), [Lucas Fellipe](https://github.comlucasfcm9)|
| 09/11/2020 | 0.7 | Tópico 6 - Visão de Processos  | [Guilherme Mendes](https://github.com/guilherme-mendes) |
| 05/11/2020 | 0.8 | Tópico 4 – Casos de Uso - Adição de Todos os Fluxos Alternativos | [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) |
| 09/11/2020 | 0.9 | Tópico 9 - Qualidade | [Guilherme Mendes](https://github.com/guilherme-mendes) |
| 11/11/2020 | 1.0 | Tópico 7 - Visão de Implementação - Diagrama de Classes e Diagrama Entidade Relacionamento | [Caio Fernandes](https://github.com/caiovfernandes), [Lucas Fellipe](https://github.comlucasfcm9) |
| 11/11/2020 | 1.1 | Tópico 8 - Tamanho e Desempenho | [Lucas Fellipe](https://github.comlucasfcm9) |
| 16/11/2020 | 1.2 | Revisão do Documento | [Lucas Fellipe](https://github.comlucasfcm9) |
| 17/11/2020 | 1.3 | Revisão dos artefatos do Documento de Arquitetura | [Guilherme Mendes](https://github.com/guilherme-mendes) |

### **1. Introdução**

#### **1.1. Finalidade**

<p align="justify"> &emsp;&emsp; Este documento oferece uma visão geral arquitetural abrangente do sistema, usando diversas visões arquiteturais para representar diferentes aspectos do sistema. O objetivo deste documento é capturar e comunicar as decisões arquiteturais significativas que foram tomadas em relação ao sistema. </p>

#### **1.2. Escopo**

<p align="justify"> &emsp;&emsp; iGado é um aplicativo que visa contribuir o gerenciamento e gestão dos bovinos que se concentram em propriedades rurais. Neste documento será detalhado os padrões arquiteturais relacionados ao aplicativo iGado desenvolvido durante a disciplina de Arquitetura e Desenho de <i>Software</i>, da Universidade de Brasília (UnB).</p>

#### **1.3. Referências**

- [https://pax-app.github.io/Wiki/#/docs/DS/dinamica-e-seminario-4-b/DAS](https://pax-app.github.io/Wiki/#/docs/DS/dinamica-e-seminario-4-b/DAS)
- [https://desenhosoftware-2018-2.github.io/wiki/docArquitetura](https://desenhosoftware-2018-2.github.io/wiki/docArquitetura)
- [https://octa-bit.github.io/ForceGamaAttack/das.html](https://octa-bit.github.io/ForceGamaAttack/das.html)
- [https://fga-eps-mds.github.io/2019.1-ADA/#/docs/project/architecture\_doc?id=documento-de-arquitetura](https://fga-eps-mds.github.io/2019.1-ADA/#/docs/project/architecture_doc?id=documento-de-arquitetura)
- https://fga-eps-mds.github.io/2019.1-Aix/projeto/2019/03/29/documento-de-arquitetura/
- Conceitos Fundamentais – Testes de Software, Semestre 1/2020
- [https://requisitos-de-software.github.io/2019.2-Wire/#/docs/modeling/user\_cases/user\_cases?id=m%c3%b3dulos-dos-casos-de-uso](https://requisitos-de-software.github.io/2019.2-Wire/#/docs/modeling/user_cases/user_cases?id=m%C3%B3dulos-dos-casos-de-uso)

#### **1.4. Visão Geral**

<p align="justify"> &emsp;&emsp;  Esse é um documento informativo sobre o <i>Software</i> iGado que está organizado no formato de tópicos e subtópicos sequenciais numerados. A ordem desses tópicos começa em 1 e termina em 9, sendo eles: Introdução; Representação Arquitetural; Metas e Restrições da Arquitetura; Visão de Casos de Uso; Visão Lógica; Visão da Implementação; Tamanho e Desempenho e Qualidade. </p>

### **2. Representação Arquitetural**

<p align="justify"> &emsp;&emsp; Modelo de representação da arquitetura e as interações estabelecidas entre os módulos, bem como a natureza dessas interações. </p>

#### **2.1 - Visão Geral**

<img src="docs/Assets/Img/Project/ArchitectureDocument/ArchitecturalRepresentation.png"> <br />


#### **2.2 - Tecnologias**

#### 2.2.1 Front End

  - **Flutter:** Flutter é o kit de ferramentas da <i>Google</i> para desenvolvimento de interfaces de usuário bonitas, com aplicações compiladas nativamente para <i>mobile</i>, <i>web</i> e <i>desktop</i> a partir de uma única base de código. A linguagem Dart é utilizada como base para essas ferramentas.
  - **Dart:** Dart é uma linguagem de programação otimizada para desenvolvimento. Será utilizada no <i>front-end</i> para desenvolvimento de algoritmos lógicos e conexões com o <i>back-end</i>.

#### 2.2.2 Back End

  - **Flask:** O Flask é um micro <i>framework</i> para Python baseado em Werkzeug, Jinja 2 e good intentions. Ao contrário de outros web <i>frameworks</i>, o Flask não tem uma camada adicional de acesso ao banco de dados, com isso, a integração com <i>toolkits</i> de banco de dados facilita o seu uso.

    Essa arquitetura será utilizada para a construção da API, que vai ser um dos pontos principais do projeto. Através da API, a aplicação irá se comunicar com a camada de <i>front-end</i> sem o conhecimento ou intervenção dos usuários, definindo comportamentos específicos de determinado objeto em uma interface.

  - **Python –** Python é uma linguagem de programação que permite você desenvolver mais rapidamente e de uma forma mais efetiva, ela será utilizada para desenvolvimento de algoritmos lógicos no <i>back-end</i>.
  - **Docker:** Ferramenta utilizada para gerar um ambiente isolado a partir da criação de contêineres que suprem as dependências do projeto, o que facilita a utilização de serviços distintos.

#### 2.2.3 Banco de Dados

  - **PostgreSQL:** É um sistema gerenciador de banco de dados <i>open-source</i> (código aberto) de objeto relacional que possui uma forte reputação de confiabilidade, robustez e desempenho. Será utilizado para armazenar os dados provenientes da API.

### **3. Metas e Restrições da Arquitetura**

#### **3.1 - Restrições**

  - O <i>software</i> deve ser desenvolvido nas tecnologias definidas no tópico 2;
  - O <i>software</i> deve rodar tanto em Android quanto em iOS;
  - O ambiente de desenvolvimento do <i>software</i> deve funcionar tanto em Windows, Linux e MacOS;
  - Para utilizar o <i>software</i> é necessário ter internet;
  - O escopo do projeto deve ser concluído até o final da disciplina.

#### **3.2 - Metas**

As metas planejadas para o aplicativo são:

  - **Portabilidade** – Deve ser possível utilizar o aplicativo tanto em sistemas Android quanto iOS.
  - **Usabilidade** - O <i>software</i> deve possuir alta aprendibilidade e inteligibilidade, para que atenda aos requisitos elicitados no formulário criado pelo grupo;
  - **Manutenibilidade –** O código e as documentações realizadas pelo grupo devem estar num nível de qualidade, seguindo os padrões de projeto e bibliografia, onde a sua manutenção seja fácil de ser realizada.

### **4. Visão de Casos de Uso**

Para representação dos Casos de Uso do sistema especificado, foram criados três diagramas referentes a módulos distintos do aplicativo, o módulo de bovinos, o módulo de manejos e o módulo de relatórios. Esses módulos serão apresentados a seguir:

#### **4.1 - Módulo de Bovinos**

**Diagrama de Casos de Uso**

<img src="docs/Assets/Img/Project/ArchitectureDocument/CattleModule.png">

**Especificação dos Casos de Uso**

| Caso de Uso | Ator | Descrição |
| --- | --- | --- |
| **UC01 –** Register Cattle | User | Este caso de uso ocorre quando o usuário registra um novo gado |
| **UC02 –** Visualize Cattle | User | Este caso de uso ocorre quando o usuário seleciona um gado para visualizar os dados |
| **UC03 –** Perform Management | User | Este caso de uso permite o usuário realizar uma manejo no bovino |
| **UC04 –** Edit Cattle | User | Este caso de uso permite o usuário editar os dados do bovino |
| **UC05 –** Delete Cattle | User | Este caso de uso permite o usuário deletar um bovino |

**Fluxo de Eventos**

**UC01** - Register Cattle

**Fluxo básico**

O usuário registra um novo gado e visualiza os dados cadastrados na tela do bovino.

**Fluxos alternativos**

**FA1 –** Perform Management

O usuário seleciona um bovino para visualizar e, após isso, seleciona a opção de realizar um manejo.

**FA2 –** Edit Cattle

O usuário seleciona um bovino para visualizar e, após isso, edita os dados daquele bovino.

**FA3 –** Delete Cattle

O usuário seleciona um bovino para visualizar e, após isso, deleta o bovino.

**4.2 - Módulo de Manejos**

**Diagrama de Casos de Uso**

<img src="docs/Assets/Img/Project/ArchitectureDocument/ManagementModule.png">

**Especificação dos Casos de Uso**

| Caso de Uso | Ator | Descrição |
| --- | --- | --- |
| **UC03 –** Perform Management | User | Este caso de uso permite o usuário realizar uma manejo no bovino |
| **UC06 –** Select desired management | User | Este caso de uso ocorre quando o usuário seleciona um manejo para realizar |
| **UC07 –** Perform reproduction management | User | Este caso de uso se refere a realização dos manejos de reprodução |
| **UC08** – Select reproduction type | User | Este caso de uso ocorre quando o usuário seleciona o tipo de reprodução realizado no manejo de reprodução |
| **UC09** – Perform weighing management | User | Este caso de uso se refere a realização dos manejos de pesagem |
| **UC10** – Inform Cattle actual status | User | Este caso de uso se refere ao usuário inserir as informações necessárias para o manejo de pesagem |
| **UC11** – Get average weight per Cattle | User | Este caso de uso se refere ao usuário gerar o manejo para um bovino específico |
| **UC12** – Get average weight per batch | User |  Este caso de uso se refere ao usuário gerar o manejo para todo um lote de bovinos |
| **UC13** – Perform sanitary management | User | Este caso de uso se refere a realização dos manejos sanitários |
| **UC14** – Select medicine | User | Este caso de uso ocorre quando o usuário seleciona o tipo de medicamento aplicado no manejo sanitário |

**Fluxo de Eventos**

**UC03** - Perform Management

**Fluxo básico**

O usuário decide realizar um manejo e seleciona o manejo que ele deseja realizar

**Fluxos alternativos**

**FA1 –** Perform reproduction management
O usuário seleciona o manejo de reprodução e então insere as informações sobre que tipo de reprodução está sendo realizada.

**FA2 –** Perform sanitary management
O usuário seleciona o manejo sanitário e então insere as informações do medicamento que será utilizado no manejo.

**FA3 –** Perform weighing management
O usuário seleciona o manejo de pesagem e então insere as informações relacionadas ao peso atual do bovino.

**FA4 –** Perform weighing management
O usuário seleciona o manejo de pesagem e então insere as informações relacionadas ao peso atual do bovino.

**FA5 –** Perform weighing management
O usuário seleciona o manejo de pesagem e então insere as informações relacionadas ao peso atual do bovino.

**FA6 –** Get average weight per cattle
O usuário durante o manejo de pesagem seleciona a opção de pegar informações de manejo de apenas um bovino.

**FA7 –** Get average weight per batch
O usuário durante o manejo de pesagem seleciona a opção de pegar informações de manejo de um lote de bovinos.

**4.3 - Módulo de Relatórios**

**Diagrama de Casos de Uso**

<img src="docs/Assets/Img/Project/ArchitectureDocument/ReportModule.png">

**Especificação dos Casos de Uso**

| Caso de Uso | Ator | Descrição |
| --- | --- | --- |
| **UC15 –** Generate report | User | Este caso de uso permite o usuário gerar um relatório|
| **UC16** – Select data report | User | Este caso de uso se refere ao usuário selecionar qual tipo de relatório quer gerar |
| **UC17** – Generate general report | User | Este caso de uso se refere ao usuário gerar o relatório geral da fazenda |
| **UC18** – Generate GMD report | User | Este caso de uso se refere ao usuário gerar o relatório com as informações do ganho de massa diário do bovino|
| **UC19** – Generate IABCZ report | User | Este caso de uso se refere ao usuário gerar o relatório com as informações indice ABCZ|
| **UC20** – Generate PMGZ report | User | Este caso de uso se refere ao usuário gerar o relatório com as informações do índice PMGZ|
| **UC21** – Select management report | User | Este caso de uso se refere ao usuário selecionar um relatório do tipo manejo |
| **UC22** – Generate reproductive management report | User | Este caso de uso se refere ao usuário gerar o relatório com as informações do manejo reprodutivo |
| **UC23** – Generate weighing management report | User | Este caso de uso se refere ao usuário gerar o relatório com as informações do manejo de pesagem|
| **UC24** – Generate sanitary management report | User | Este caso de uso se refere ao usuário gerar o relatório com as informações do manejo sanitário |

**Fluxo de Eventos**

**UC15** - Generate report

**Fluxo básico**

O usuário decide gerar um relatório e seleciona o tipo de relatório que será gerado

**Fluxos alternativos**

**FA1 –** Generate geral report
O usuário seleciona a opção de gerar o relatório geral com todas as informações da fazenda.

**FA2 –** Generate GMD report
O usuário seleciona a opção de gerar o relatório com informações da métrica GMD (Ganho de Massa Diária).

**FA3 –** Generate IABCZ report
O usuário seleciona a opção de gerar o relatório com informações do índice ABCZ.

**FA4 –** Generate PMGZ report
O usuário seleciona a opção de gerar o relatório com informações do índice PMGZ.

**FA5 –** Select management reprot
O usuário seleciona a opção de gerar relatório de manejos e pode selecionar um dos relatórios disponíveis.

**FA6 –** Generate reproductive management report
O usuário seleciona a opção de gerar o relatório com as informações do manejo de reprodução.

**FA7 –** Generate weighing management report
O usuário seleciona a opção de gerar o relatório com as informações do manejo de pesagem.

**FA8 –** Generate sanitary management report
O usuário seleciona a opção de gerar o relatório com as informações do manejo sanitário.

### **5. Visão Lógica**

<p align="justify"> &emsp;&emsp; A visão lógica descreve como o sistema é estruturado, em termos de unidade e implementação. Mostra como está a organização conceitual do sistema em termos de camadas, pacotes, classes e interfaces. O relacionamento entre os elementos mostra as dependências, as realizações de interface, os relacionamento parte-todo e assim por diante. </i>

#### **5.1 Diagrama de Pacotes**

<p align="justify"> &emsp;&emsp; Os diagramas de pacotes mostram a interação entre as relações das pastas e seus arquivos. Tem como objetivo estruturar hierarquicamente as pastas que compõem o projeto. </i>

A sua rastreabilidade pode ser acompanhada [aqui](https://unbarqdsw.github.io/2020.1_G13_iGado/#/docs/Modeling/PackageDiagram).

<img src="docs/Assets/Img/Modeling/PackageDiagram/PackageDiagramV2.0.png"> <br />

<br>
<br>
<br>
<br>


### **6. Visão de Processos**

#### **6.1 Visão Geral**

<p align="justify"> &emsp;&emsp; A Visão de Processos tem como objetivo descrever a estrutura de processos do sistema. Tendo como base uma visualização em sequência para mostrar como será feito o modelo do projeto. </p>

#### **6.2 Diagrama de Sequência**

<p align="justify"> &emsp;&emsp; O Diagrama de Sequência é uma das soluções que a UML oferece, de maneira dinâmica para detalhar os fluxos de vida do sistema em desenvolvimento. O principal foco da elaboração desse diagrama é descrever sobre a interação entre componentes do sistema, processos e módulos que, de alguma maneira, vivem simultaneamente e trocam mensagens entre si. Os ciclos de vida podem ser classes, atores ou até mesmo abstrações que ocorrem entre as classes. </p>

#### **6.2.1 Cadastro de Usuário**

<p align="justify"> &emsp;&emsp; Detalha o módulo de Cadastro de Usuário do sistema, mostrando como funcionará o cadastro de um usuário, sua fazer e seus funcionários, respectivamente. </p>

<img src="docs/Assets/Img/Modeling/SequenceDiagram/SequenceDiagram-RegistroELoginV2.png">

<a href="docs/Assets/Img/Modeling/SequenceDiagram/SequenceDiagram-RegistroELoginV2.png"> Clique aqui para ampliar</a>

#### **6.2.2 Cadastro de Bovino**

<p align="justify"> &emsp;&emsp; Detalha o módulo de Cadastro de Bovino, demonstrando como este fluxo funcionará no app, com o proprietário podendo cadastrar diferentes tipos de bovinos (de corte, de leite e bezerros). </p>

<img src="docs/Assets/Img/Modeling/SequenceDiagram/SequenceDiagram-CadastroDeBovinoV2.png">

<a href="docs/Assets/Img/Modeling/SequenceDiagram/SequenceDiagram-CadastroDeBovinoV2.png"> Clique aqui para ampliar</a>

#### **6.2.3 Manejo**

<p align="justify"> &emsp;&emsp; Demonstra o módulo de Manejo Bovino, detalhando os diferentes tipos de manejo. </p>

<img src="docs/Assets/Img/Modeling/SequenceDiagram/SequenceDiagram-ManejoV2.png">

<a href="docs/Assets/Img/Modeling/SequenceDiagram/SequenceDiagram-ManejoV2.png"> Clique aqui para ampliar</a>

#### **6.2.4 Estoque de Insumos**

<p align="justify"> &emsp;&emsp; Detalha o módulo Estoque de Insumos, que será responsável por gerenciar produtos de uma fazenda. </p>

<img src="docs/Assets/Img/Modeling/SequenceDiagram/SequenceDiagram-EstoqueDeInsumosV2.png">

<a href="docs/Assets/Img/Modeling/SequenceDiagram/SequenceDiagram-EstoqueDeInsumosV2.png"> Clique aqui para ampliar</a>

#### **6.2.5 Relatório**
<p align="justify"> &emsp;&emsp; Demonstra o módulo de *Relatório*, que se trata de uma funcionalidade para auxiliar o Proprietário na tomada de decisão. Trazendo informções a partir de métricas utilizando os dados de seus recursos. </p>

<img src="docs/Assets/Img/Modeling/SequenceDiagram/SequenceDiagram-RelatórioV2.png">

<a href="docs/Assets/Img/Modeling/SequenceDiagram/SequenceDiagram-RelatórioV2.png"> Clique aqui para ampliar</a>


### **7. Visão de Implementação**

#### **7.1 Visão Geral**
<p align="justify"> &emsp;&emsp; A visão de implementação mostra como o sistema proposto será implementado. Uma das suas principais características é a visao geral do Diagrama de Classes final do projeto. </p>

#### **7.2 Diagrama de Classes**
<p align="justify"> &emsp;&emsp; O Diagrama de Classes é uma representação da estrutura e relações das classes que servem de modelo para os objetos. Consiste em um conjunto de objetos com as mesmas características. Dessa forma, consegue-se identificar os objetos e agrupá-los, de forma a encontrar suas respectivas classes. </p>

A sua rastreabilidade pode ser acompanhada [neste link](https://unbarqdsw.github.io/2020.1_G13_iGado/#/docs/Modeling/ClassDiagram)

<img src="https://unbarqdsw.github.io/2020.1_G13_iGado/docs/Assets/Img/Modeling/ClassDiagram/ClassDiagramV1.2.png"> <br />


#### **7.3 Diagrama de Entidade Relacionamento**
<p align="justify"> &emsp;&emsp; O Diagrama de Entidade-Relacionamento (DER) é um tipo de fluxograma que ilustra como “entidades”, como pessoas, objetos ou conceitos, se relacionam entre si dentro de um sistema. Diagramas de Entidade Relacionamento são mais utilizados para projetar ou depurar bancos de dados relacionais nas áreas de engenharia de software. Também conhecidos como DERs, ou modelos ER, usam um conjunto definido de símbolos, tais como retângulos, diamantes, ovais e linhas de conexão para representar a interconectividade de entidades, relacionamentos e seus atributos. Eles espelham estruturas gramaticais, onde entidades são substantivos e relacionamentos são verbos.</p>

A sua rastreabilidade pode ser acompanhada [aqui](https://unbarqdsw.github.io/2020.1_G13_iGado/#/docs/Modeling/DatabaseModeling).

<img src="docs/Assets/Img/Modeling/DatabaseModeling/DER_v1.png"> <br />


### **8. Tamanho e Desempenho**

#### **8.1 Visão Geral**

<p align="justify"> &emsp;&emsp; Descreve os principais objetivos de desempenho do <i>software</i> assim como as principais características de dimensionamento do <i>software</i> que impactam na arquitetura do aplicativo. </p>

#### **8.2 Requisitos Mínimos**

* Sistemas operacionais: Android e iOS
* É necessário possuir internet móvel ou Wi-Fi para utilizar o <i>Software</i>.
* O ambiente de desenvolvimento deve funcionar tanto em Windows, Linux e MacOS;
* iOS 12.0 ou superior;
* Android 10.0 ou superior;


### **9. Qualidade**

Descrição de como a arquitetura do <i>software</i> contribui para todos os recursos (exceto a funcionalidade) do sistema: extensibilidade, confiabilidade, portabilidade e assim por diante.

#### **9.1 NFR**

<p align="justify"> &emsp;&emsp; A fim de rastrear requisitos não funcionais, o NFR mostram impactos que um <i>hardgoal</i> causa em um <i>softgoal</i>, deixando explícito a rastreabilidade e propósito de uma determiada <i>feature</i>, deixando claro os recursos do sistema de qualidade, como usabilidade, eficiência e etc.</p>

<img src="docs/Assets/Img/Project/ArchitectureDocument/nfr.png">

<a href="docs/Assets/Img/Project/ArchitectureDocument/nfr.png"> Clique aqui para ampliar</a>
