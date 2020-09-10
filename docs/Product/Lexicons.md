# Léxicos

|    Data    | Versão |         Descrição         |           Autor(es)           |
| :--------: | :----: | :-----------------------: | :---------------------------: |
| 09/09/2020 |  1.0   | Criação do documento dos Léxicos Gerais |[Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes) e [Lucas Fellipe](https://github.com/lucasfcm9) |

<p align="justify"> &emsp;&emsp; Léxico é definido como um conjunto dos vocábulos de uma língua, dispostos em ordem alfabética e com as respectivas significações. Uma notação na modelagem de requisitos que usa a descrição de termos via léxico é o LAL (Léxico Ampliado da Linguagem). </p>

<p align="justify"> &emsp;&emsp; Trata-se de uma técnica que descreve os símbolos de uma linguagem. Esses símbolos são descritos com noções e impactos. A noção significa o símbolo, que pode ser colocado no sentido denotativo da linguagem. Já o impacto descreve o efeito/uso/ocorrência do símbolo na aplicação ou do efeito de algo na aplicação sobre o símbolo, que pode ser colocado no sentido conotativo da linguagem. </p> 

<p align="justify"> &emsp;&emsp; Os léxicos podem ser definidos em objetos, estados, sujeitos e verbos. </p>

| **Nome**          | <Nome do Léxico>                   |
| ----------------- | ---------------------------------- |
| **Classificação** | <Verbo, Sujeito, Objeto ou Estado> |
| **Sinônimos**     | <Sinônimos do Léxico>              |
| **Noção**         | <Descrição do Léxico>              |
| **Impacto**       | <Impacto do léxico na aplicação>   |

### Vacina
| **Nome**          | Vacina                                                       |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | -                                                            |
| **Noção**         | Preparação biológica que fornece imunidade adquirida ativa para uma doença particular |
| **Impacto**       | Um [bovino](/docs/Product/Lexicons?id=bovino) pode ser vacinado <br />Um [funcionário](/docs/Product/Lexicons?id=funcionário) pode aplicar a vacina em um determinado [bovino](/docs/Product/Lexicons?id=bovino) <br />O [proprietário](/docs/Product/Lexicons?id=proprietário) pode gerenciar o controle da quantidade de [vacinas](/docs/Product/Lexicons?id=vacina) |

### Bovino
| **Nome**          | Bovino                                                     |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Boi, Vaca, Gado, Animal, Rebanho                             |
| **Noção**         | Objeto que será cadastrado no banco de dados no qual as suas informações serão extraídas |
| **Impacto**       | Um [bovino](/docs/Product/Lexicons?id=bovino) pode ser cadastrado no aplicativo <br />O cadastro do [bovino](/docs/Product/Lexicons?id=bovino) será realizado por um [funcionário](/docs/Product/Lexicons?id=funcionário) ou pelo [proprietário](/docs/Product/Lexicons?id=proprietário)<br />As informações do [bovino](/docs/Product/Lexicons?id=bovino) poderão ser visualizadas a qualquer momento<br />As informações do [bovino](/docs/Product/Lexicons?id=bovino) poderão ser alteradas <br />Geração de [relatórios](/docs/Product/Lexicons?id=relatórios) com os dados referentes aos [bovinos](/docs/Product/Lexicons?id=bovino) |

### Funcionário
| **Nome**          | Funcionário                                                  |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Sujeito                                                      |
| **Sinônimos**     | Empregado rural, Caseiro                                     |
| **Noção**         | [Funcionário](/docs/Product/Lexicons?id=funcionário) que trabalha na [fazenda](/docs/Product/Lexicons?id=fazenda) responsável por gerenciar o [gado](/docs/Product/Lexicons?id=bovino) |
| **Impacto**       | O [funcionário](/docs/Product/Lexicons?id=funcionário) poderá coletar dados dos [bovinos](/docs/Product/Lexicons?id=bovino)  <br />O [funcionário](/docs/Product/Lexicons?id=funcionário) poderá inserir essas informações no aplicativo <br />Um [funcionário](/docs/Product/Lexicons?id=funcionário) pode cadastrar um [bovino](/docs/Product/Lexicons?id=bovino) <br />Um [funcionário](/docs/Product/Lexicons?id=funcionário) pode editar seus dados e dados do [bovino](/docs/Product/Lexicons?id=bovino) <br />Um [funcionário](/docs/Product/Lexicons?id=funcionário) pode gerar [relatórios](/docs/Product/Lexicons?id=relatórios) referentes aos [bovinos](/docs/Product/Lexicons?id=bovino) |

### Proprietário
| **Nome**          | [Proprietário](/docs/Product/Lexicons?id=proprietário)                                                 |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Sujeito                                                      |
| **Sinônimos**     | Fazendeiro, Dono da [fazenda](/docs/Product/Lexicons?id=fazenda), Pecuarista                      |
| **Noção**         | Responsável por gerenciar a [fazenda](/docs/Product/Lexicons?id=fazenda)                          |
| **Impacto**       | [Proprietário](/docs/Product/Lexicons?id=proprietário) pode coletar dados dos [bovinos](/docs/Product/Lexicons?id=bovino)<br />[Proprietário](/docs/Product/Lexicons?id=proprietário) pode inserir e remover esses dados no aplicativo <br />[Proprietário](/docs/Product/Lexicons?id=proprietário) pode visualizar seus gastos e ter um controle sobre eles <br />[Proprietário](/docs/Product/Lexicons?id=proprietário) pode editar seus dados e dados dos [bovinos](/docs/Product/Lexicons?id=bovino) <br />[Proprietário](/docs/Product/Lexicons?id=proprietário) pode gerar [relatórios](/docs/Product/Lexicons?id=relatórios) referentes aos [bovinos](/docs/Product/Lexicons?id=bovino) e aos seus gastos<br />[Proprietário](/docs/Product/Lexicons?id=proprietário) pode adicionar mais de uma [fazenda](/docs/Product/Lexicons?id=fazenda) |

### Relatório
| **Nome**          | Relatório                                                    |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Informações, Exposição de dados.                             |
| **Noção**         | Conjunto de informações utilizado para reportar resultados coletados da [fazenda](/docs/Product/Lexicons?id=fazenda) |
| **Impacto**       | Gerar [relatórios](/docs/Product/Lexicons?id=relatórios) sobre o estoque de alimentos, água, [vacinas](/docs/Product/Lexicons?id=vacina), etc... <br />Gerar [relatórios](/docs/Product/Lexicons?id=relatórios) sobre os [bovinos](/docs/Product/Lexicons?id=bovino) <br />Gerar [relatórios](/docs/Product/Lexicons?id=relatórios) sobre os gastos |

### Manejo
| **Nome**          | Manejo                         |
| ----------------- | ------------------------------ |
| **Classificação** | Verbo                          |
| **Sinônimos**     | Manipulação do [gado](/docs/Product/Lexicons?id=bovino), Manuseio. |
| **Noção**         | Transporte dos [animais](/docs/Product/Lexicons?id=bovino)        |
| **Impacto**       | Gerar [relatórios](/docs/Product/Lexicons?id=relatórios) a respeito dos vários tipos de [manejo](/docs/Product/Lexicons?id=manejo)                               |

### Fazenda
| **Nome**          | Fazenda                                                      |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | [Propriedade rural](/docs/Product/Lexicons?id=proprietário), rancho, sítio                             |
| **Noção**         | [Propriedade rural](/docs/Product/Lexicons?id=proprietário) de lavoura ou de criação de gado           |
| **Impacto**       | Cadastrar uma [fazenda](/docs/Product/Lexicons?id=fazenda) <br />Editar os dados referentes a uma [fazenda](/docs/Product/Lexicons?id=fazenda) <br />Adicionar um [proprietário](/docs/Product/Lexicons?id=proprietário) para a [fazenda](/docs/Product/Lexicons?id=fazenda) |

### Pasto
| **Nome**          | Pasto                                                        |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Alimento [bovino](/docs/Product/Lexicons?id=bovino), ração                                       |
| **Noção**         | Vegetação utilizada para a alimentação do [gado](/docs/Product/Lexicons?id=bovino) e por extensão ou terreno onde o [gado](/docs/Product/Lexicons?id=bovino) é deixado para se alimentar. |
| **Impacto**       | Cadastrar uma [fazenda](/docs/Product/Lexicons?id=fazenda) <br />Editar os dados referentes a uma [fazenda](/docs/Product/Lexicons?id=fazenda) <br />Cadastrar um [bovino](/docs/Product/Lexicons?id=bovino) <br />Coletar dados do [bovino](/docs/Product/Lexicons?id=bovino) <br />Geração de [relatórios](/docs/Product/Lexicons?id=relatórios) |

### GMD
| **Nome**          | GMD                                                          |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | [Ganho de Massa Diária](/docs/Product/Lexicons?id=gmd)                                        |
| **Noção**         | Índice referente ao ganho de massa diário de um [bovino](/docs/Product/Lexicons?id=bovino)       |
| **Impacto**       | Cálculo para saber o [Ganho de Massa Diário](/docs/Product/Lexicons?id=gmd) de um [bovino](/docs/Product/Lexicons?id=bovino) <br />[GMD](/docs/Product/Lexicons?id=gmd) é uma métrica para a geração de [relatórios](/docs/Product/Lexicons?id=relatórios) |

### RGD
| **Nome**          | RGD                                                          |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Registro genealógico definitivo                              |
| **Noção**         | Condição para que os filhos desse [gado](/docs/Product/Lexicons?id=bovino) não apresentem nenhuma desclassificação racial |
| **Impacto**       | [RGD](/docs/Product/Lexicons?id=rgd) é uma métrica para a geração de [relatórios](/docs/Product/Lexicons?id=relatórios)               |

### Hectare
| **Nome**          | Hectare                                                      |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Área, unidade de medida                                      |
| **Noção**         | Unidade de medida de área equivalente a 100 ares ou a 10 000 metros quadrados |
| **Impacto**       | Cadastrar [fazenda](/docs/Product/Lexicons?id=fazenda)<br />Geração de [relatórios](/docs/Product/Lexicons?id=relatórios) <br />Lucro Por [Hectare](/docs/Product/Lexicons?id=hectare) Por Ano |

### Taxa de Lotação
| **Nome**          | Taxa de Lotação                                              |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | -                                                             |
| **Noção**         | A [taxa de lotação](/docs/Product/Lexicons?id=taxa-de-lotacao) é definida pelo número de animais dividido pela área pastejada |
| **Impacto**       | Cadastrar [fazenda](/docs/Product/Lexicons?id=fazenda) <br />Cadastrar [gado](/docs/Product/Lexicons?id=bovino) <br />Geração de [relatórios](/docs/Product/Lexicons?id=relatórios) |

### Prenhez
| **Nome**          | Prenhez                                                      |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Estado                                                       |
| **Sinônimos**     | Gravidez, fetação, gestação                                  |
| **Noção**         | Estado em que a [vaca](/docs/Product/Lexicons?id=bovino) está prenha                             |
| **Impacto**       | Adicionar esse dado como verdadeiro se a [vaca](/docs/Product/Lexicons?id=bovino) estiver [prenha](/docs/Product/Lexicons?id=prenhez) <br /> O [proprietário](/docs/Product/Lexicons?id=proprietário) pode saber se a vaca está [prenha](/docs/Product/Lexicons?id=prenhez) ou não <br />A [prenhez](/docs/Product/Lexicons?id=prenhez) pode trazer um custo benefício vantajoso ao [produtor rural](/docs/Product/Lexicons?id=proprietário). |

### Gado de Corte 
| **Nome**          | Gado de Corte                                                |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Pecuária de corte                                            |
| **Noção**         | O [gado](/docs/Product/Lexicons?id=bovino) de corte é o [gado](/docs/Product/Lexicons?id=bovino) criado para a produção de carne.    |
| **Impacto**       | Adicionar [gado](/docs/Product/Lexicons?id=bovino) de corte para obter metricas na geracão de [relatórios](/docs/Product/Lexicons?id=relatórios) e lucros. |

### Gado de Leite 
| **Nome**          | Gado de Leite                                                |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Pecuária de leite                                            |
| **Noção**         | O [gado](/docs/Product/Lexicons?id=bovino) de leite é o [gado](/docs/Product/Lexicons?id=bovino) criado para a produção de leite.    |
| **Impacto**       | Adicionar [gado](/docs/Product/Lexicons?id=bovino) de leite para obter métricas na geração de [relatórios](/docs/Product/Lexicons?id=relatórios) e lucros com a venda de produtos lácteos. |

### Taxa de Desmama   
| **Nome**          | Taxa de Desmama                                              |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | -                                                            |
| **Noção**         | Representa o total de [bovinos](/docs/Product/Lexicons?id=bovino) desmamados em relação às [vacas](/docs/Product/Lexicons?id=bovino) expostas em reprodução dentro de um determinado período. |
| **Impacto**       | Geração de [relatórios](/docs/Product/Lexicons?id=relatórios)                                              |

 