# **Nome do Projeto**

# **Documento de Arquitetura de Software**

**Versão \&lt;1.0\&gt;**

_[Observação: O template a seguir é fornecido para uso com o Rational Unified Process (RUP). O texto em azul exibido entre colchetes e em itálico (style=InfoBlue) foi incluído para orientar o autor e deve ser excluído antes da publicação do documento. Um parágrafo digitado após esse estilo será automaticamente definido como normal (style=Body Text).]_

_[Para personalizar campos automáticos no Microsoft Word (que exibem um fundo cinza quando selecionados), escolha File\&gt;Properties e substitua os campos Title, Subject e Company pelas informações apropriadas para este documento. Depois de fechar a caixa de diálogo, para atualizar os campos automáticos no documento inteiro, selecione Edit\&gt;Select All (ou Ctrl-A) e pressione F9 ou simplesmente clique no campo e pressione F9. Isso deve ser feito separadamente para Cabeçalhos e Rodapés. Alt-F9 alterna entre a exibição de nomes de campos e do conteúdo dos campos. Consulte a ajuda do Word para obter mais informações sobre como trabalhar com campos.]_

## **Histórico da Revisão**

| **Data** | **Versão** | **Descrição** | **Autor** |
| --- | --- | --- | --- |
| 04/11/2020 | 0.1 | Criação do documento | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 04/11/2020 | 0.2 | Tópico 1 - introdução | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 04/11/2020 | 0.3 | Tópico 2 - representação arquitetural | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 04/11/2020 | 0.4 | Tópico 3 – metas e restrições de arquitetura | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 05/11/2020 | 0.5.1 | Tópico 4 – Casos de Uso - Diagramas e Fluxos básicos | [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) |
| 05/11/2020 | 0.5.2 | Tópico 4 – Casos de Uso - Descrição dos casos de uso e fluxos alternativos | [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) |
| 09/11/2020 | 0.6 | Tópico 5 – Lógico:  Diagrama de classes e de Pacotes | [Caio Fernandes](https://github.com/caiovfernandes)|

## **Índice Analítico**

1. Introdução

    1.1 Finalidade

    1.2 Escopo

    1.3 Definições, Acrônimos e Abreviações

    1.4 Referências

    1.5 Visão Geral

2. Representação Arquitetural

3. Metas e Restrições da Arquitetura

4. Visão de Casos de Uso

    4.1 Realizações de Casos de Uso

5. Visão Lógica

    5.1 Visão Geral

    5.2 Pacotes de Design Significativos do Ponto de Vista da Arquitetura

6. Visão de Processos

7. Visão de Implantação

8. Visão da Implementação

    8.1 Visão Geral

    8.2 Camadas

9. Visão de Dados (opcional)

10. Tamanho e Desempenho

11. Qualidade

## **Documento de Arquitetura de Software**

### **1. Introdução**

#### **1.1. Finalidade**

Este documento oferece uma visão geral arquitetural abrangente do sistema, usando diversas visões arquiteturais para representar diferentes aspectos do sistema. O objetivo deste documento é capturar e comunicar as decisões arquiteturais significativas que foram tomadas em relação ao sistema.

#### **1.2. Escopo**

IGado é um aplicativo que visa contribuir o gerenciamento e gestão dos bovinos que se concentram em propriedades rurais. Neste documento será detalhado os padrões arquiteturais relacionados ao aplicativo iGado desenvolvido durante a disciplina de Arquitetura e Desenho de software, da Universidade de Brasília.

#### **1.3. Referências**

- [https://pax-app.github.io/Wiki/#/docs/DS/dinamica-e-seminario-4-b/DAS](https://pax-app.github.io/Wiki/#/docs/DS/dinamica-e-seminario-4-b/DAS)
- [https://desenhosoftware-2018-2.github.io/wiki/docArquitetura](https://desenhosoftware-2018-2.github.io/wiki/docArquitetura)
- [https://octa-bit.github.io/ForceGamaAttack/das.html](https://octa-bit.github.io/ForceGamaAttack/das.html)
- [https://fga-eps-mds.github.io/2019.1-ADA/#/docs/project/architecture\_doc?id=documento-de-arquitetura](https://fga-eps-mds.github.io/2019.1-ADA/#/docs/project/architecture_doc?id=documento-de-arquitetura)
- https://fga-eps-mds.github.io/2019.1-Aix/projeto/2019/03/29/documento-de-arquitetura/
- Conceitos Fundamentais – Testes de Software, Semestre 1/2020
- [https://requisitos-de-software.github.io/2019.2-Wire/#/docs/modeling/user\_cases/user\_cases?id=m%c3%b3dulos-dos-casos-de-uso](https://requisitos-de-software.github.io/2019.2-Wire/#/docs/modeling/user_cases/user_cases?id=m%C3%B3dulos-dos-casos-de-uso)

#### **1.4. Visão Geral**

Esse é um documento informativo sobre o Software iGado que está organizado no formato de tópicos e subtópicos sequenciais numerados. A ordem desses tópicos começa em 1 e termina em 7, sendo eles: Introdução; Representação Arquitetural; Metas e Restrições da Arquitetura; Visão de Casos de Uso; Visão Lógica; Visão da Implementação; Tamanho e Desempenho e Qualidade.  

### **2. Representação Arquitetural**

Modelo de representação da arquitetura e as interações estabelecidas entre os módulos, bem como a natureza dessas interações.

#### **2.1 - Visão Geral**

<img src="docs/Assets/Img/Project/ArchitectureDocument/ArchitecturalRepresentation.png"> <br />


#### **2.2 - Tecnologias**

#### 2.2.1 Front End

  - **Flutter:** Flutter é o kit de ferramentas da Google para desenvolvimento de interfaces de usuário bonitas, com aplicações compiladas nativamente para mobile, web e desktop a partir de uma única base de código. A linguagem Dart é utilizada como base para essas ferramentas.
  - **Dart –** Dart é uma linguagem de programação otimizada para desenvolvimento. Será utilizada no front-end para desenvolvimento de algoritmos lógicos e conexões com o back-end.

#### 2.2.2 Back End

  - **Flask:** O Flask é um micro framework para Python baseado em Werkzeug, Jinja 2 e good intentions. Ao contrário de outros web frameworks, o Flask não tem uma camada adicional de acesso ao banco de dados, com isso, a integração com toolkits de banco de dados facilita o seu uso.

    Essa arquitetura será utilizada para a construção da API, que vai ser um dos pontos principais do projeto. Através da API, a aplicação irá se comunicar com a camada de Front-End sem o conhecimento ou intervenção dos usuários, definindo comportamentos específicos de determinado objeto em uma interface.

  - **Python –** Python é uma linguagem de programação que permite você desenvolver mais rapidamente e de uma forma mais efetiva, ela será utilizada para desenvolvimento de algoritmos lógicos no back-end.
  - **Docker:** Ferramenta utilizada para gerar um ambiente isolado a partir da criação de containers que suprem as dependências do projeto, o que facilita a utilização de serviços distintos.

#### 2.2.3 Banco de Dados

  - **PostgreSQL:** É um sistema gerenciador de banco de dados _open-source_ (código aberto) de objeto relacional que possui uma forte reputação de confiabilidade, robustez e desempenho. Será utilizado para armazenar os dados provenientes da API.

_[Esta seção descreve qual é a arquitetura de software do sistema atual e como ela é representada. Da_ _ **Visão de Casos de Uso** __,_ _ **Visão**__ **Lógica** __,_ _ **Visão de Processos**__ ,_ _ **Visão de** __**Implantação** _ _e_ _ **Visão de**__ **Implementação** __, enumera as visões necessárias e, para cada visão, explica quais tipos de elementos de modelo ela contém.]_

### **3. Metas e Restrições da Arquitetura**

_[Esta seção descreve os requisitos e objetivos do software que têm algum impacto sobre a arquitetura; por exemplo, segurança, garantia, privacidade, uso de um produto desenvolvido internamente e pronto para ser usado, portabilidade, distribuição e reutilização. Ela também captura as restrições especiais que podem ser aplicáveis: estratégia de design e implementação, ferramentas de desenvolvimento, estrutura das equipes, cronograma, código-fonte legado e assim por diante.]_

#### **3.1 - Restrições**

  - O software deve ser desenvolvido nas tecnologias definidas no tópico 2;
  - O software deve rodar tanto em Android quanto em iOS;
  - O ambiente de desenvolvimento do software deve funcionar tanto em Windows, Linux e MacOS;
  - Para utilizar o software é necessário ter internet;
  - O escopo do projeto deve ser concluído até o final da disciplina.

#### **3.2 - Metas**

As metas planejadas para o aplicativo são:

  - **Portabilidade** – Deve ser possível utilizar o aplicativo tanto em sistemas Android quanto IOs
  - **Usabilidade** - O software deve possuir alta aprendibilidade e inteligibilidade, para que atenda aos requisitos elicitados no formulário criado pelo grupo;
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

**FA1 –** Fluxo alternativo

Descrição do Fluxo alternativo

**4.2 - Módulo de Manejos**

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
| **UC23** – Generate weighing management report | User |Este caso de uso se refere ao usuário gerar o relatório com as informações do manejo de pesagem|
| **UC24** – Generate sanitary management report | User |Este caso de uso se refere ao usuário gerar o relatório com as informações do manejo sanitário |

**Fluxo de Eventos**

**UC15** - Generate report

**Fluxo básico**

O usuário decide gerar um relatório e seleciona o tipo de relatório que será gerado

**Fluxos alternativos**

**FA1 –** Fluxo alternativo

Descrição do Fluxo alternativo

### **5. Visão Lógica**

A visão lógica descreve como o sistema é estruturado, em termos de unidade e implementação. Mostra como está a organização conceitual do sistema em termos de camadas, pacotes, classes e interfaces. O relacionamento entre os elementos mostra as dependências, as realizações de interface, os relacionamento parte-todo e assim por diante.  

#### **5.1 Diagrama de Pacotes** 

Os diagramas de pacotes mostram a interação entre as relações das pastas e seus arquivos. Tem como objetivo estruturar hierarquicamente as pastas que compõem o projeto. 

A sua rastreabilidade pode ser acompanhada [neste link](https://unbarqdsw.github.io/2020.1_G13_iGado/#/docs/Modeling/PackageDiagram)

<img src="docs/Assets/Img/Modeling/PackageDiagram/PackageDiagramV2.0.png"> <br />

<br>
<br>
<br>
<br>

#### **5.2 Diagrama de Classes** 
O Diagrama de Classes é uma representação da estrutura e relações das classes que servem de modelo para os objetos. Consiste em um conjunto de objetos com as mesmas características. Dessa forma, consegue-se identificar os objetos e agrupá-los, de forma a encontrar suas respectivas classes.

A sua rastreabilidade pode ser acompanhada [neste link](https://unbarqdsw.github.io/2020.1_G13_iGado/#/docs/Modeling/ClassDiagram)

<img src="https://unbarqdsw.github.io/2020.1_G13_iGado/docs/Assets/Img/Modeling/ClassDiagram/ClassDiagramV1.2.png"> <br />

#### **5.3 Diagrama de Entidade Relacionamento**
 O Diagrama de Entidade-Relacionamento (DER) é um tipo de fluxograma que ilustra como “entidades”, como pessoas, objetos ou conceitos, se relacionam entre si dentro de um sistema. Diagramas de Entidade Relacionamento são mais utilizados para projetar ou depurar bancos de dados relacionais nas áreas de engenharia de software. Também conhecidos como DERs, ou modelos ER, usam um conjunto definido de símbolos, tais como retângulos, diamantes, ovais e linhas de conexão para representar a interconectividade de entidades, relacionamentos e seus atributos. Eles espelham estruturas gramaticais, onde entidades são substantivos e relacionamentos são verbos.

A sua rastreabilidade pode ser acompanhada [neste link](https://unbarqdsw.github.io/2020.1_G13_iGado/#/docs/Modeling/DatabaseModeling)

<img src="docs/Assets/Img/Modeling/DatabaseModeling/DER_v1.png"> <br />

### **6. Visão de Processos**

_[Esta seção descreve a decomposição do sistema em processos leves (threads simples de controle) e processos pesados (agrupamentos de processos leves). Organize a seção em grupos de processos que se comunicam ou interagem. Descreva os modos principais de comunicação entre processos, como transmissão de mensagens e interrupções.]_


### **7. Tamanho e Desempenho**

_[Uma descrição das principais características de dimensionamento do software que têm um impacto na arquitetura, bem como as restrições do desempenho desejado.]_

### **8. Qualidade**

_[Uma descrição de como a arquitetura do software contribui para todos os recursos (exceto a funcionalidade) do sistema: extensibilidade, confiabilidade, portabilidade e assim por diante. Se essas características possuírem significado especial, como implicações de segurança, garantia ou privacidade, elas deverão ser delineadas claramente.]_