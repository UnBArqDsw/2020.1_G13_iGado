# Léxicos

|    Data    | Versão |         Descrição         |           Autor(es)           |
| :--------: | :----: | :-----------------------: | :---------------------------: |
| 09/09/2020 |  1.0   | Criação do documento dos Léxicos Gerais |[Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 28/09/2020 |  1.1   | Adição das referências e revisão dos léxicos: Vacina, Bovino, Funcionário, Proprietário, Relatório, Fazenda, Pasto, Hectare, Taxa de Lotação, Prenhez, Gado de Corte, Gado de Leite | [Iuri Severo](http://github.com/iurisevero) |
| 29/09/2020 |  1.2   | Adição do léxico Insumo e revisão dos léxicos: Manejar, GMD e RGD | [Iuri Severo](http://github.com/iurisevero) |

<p align="justify"> &emsp;&emsp; Léxico é definido como um conjunto dos vocábulos de uma língua, dispostos em ordem alfabética e com as respectivas significações. Uma notação na modelagem de requisitos que usa a descrição de termos via léxico é o LAL (Léxico Ampliado da Linguagem). </p>

<p align="justify"> &emsp;&emsp; Trata-se de uma técnica que descreve os símbolos de uma linguagem. Esses símbolos são descritos com noções e impactos. A noção significa o símbolo, que pode ser colocado no sentido denotativo da linguagem. Já o impacto descreve o efeito/uso/ocorrência do símbolo na aplicação ou do efeito de algo na aplicação sobre o símbolo, que pode ser colocado no sentido conotativo da linguagem. </p> 

<p align="justify"> &emsp;&emsp; Os léxicos podem ser definidos em objetos, estados, sujeitos e verbos. </p>

| **Nome**          | <Nome do Léxico>                   |
| ----------------- | ---------------------------------- |
| **Classificação** | {Verbo, Sujeito, Objeto, Estado} |
| **Sinônimos**     | Sinônimos do Léxico              |
| **Noção**         | Significado do símbolo              |
| **Impacto**       | Efeito, uso ou ocorrência do símbolo na aplicação  |

### Vacina
| **Nome**          | Vacina                                                       |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | -                                                            |
| **Noção**         | Preparação biológica que fornece imunidade adquirida ativa para uma doença particular |
| **Impacto**       | Um [bovino](/docs/Product/Lexicons?id=bovino) pode ser vacinado <br />Um [funcionário](/docs/Product/Lexicons?id=funcionário) pode aplicar a vacina em um determinado [bovino](/docs/Product/Lexicons?id=bovino) <br />O [proprietário](/docs/Product/Lexicons?id=proprietário) pode gerenciar o controle da quantidade de [vacinas](/docs/Product/Lexicons?id=vacina) por meio dos [insumos](/docs/Product/Lexicons?id=insumo) |

### Bovino
| **Nome**          | Bovino                                                     |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Boi, Vaca, Gado, Animal, Rebanho                             |
| **Noção**         | Objeto que será cadastrado no banco de dados do qual as suas informações serão extraídas |
| **Impacto**       | Um [bovino](/docs/Product/Lexicons?id=bovino) pode ser cadastrado no aplicativo <br />O cadastro do [bovino](/docs/Product/Lexicons?id=bovino) será realizado por um [funcionário](/docs/Product/Lexicons?id=funcionário) ou pelo [proprietário](/docs/Product/Lexicons?id=proprietário)<br />As informações do [bovino](/docs/Product/Lexicons?id=bovino) poderão ser visualizadas a qualquer momento<br />As informações do [bovino](/docs/Product/Lexicons?id=bovino) poderão ser alteradas <br />Geração de [relatórios](/docs/Product/Lexicons?id=relatório) com os dados referentes aos [bovinos](/docs/Product/Lexicons?id=bovino) |

### Funcionário
| **Nome**          | Funcionário                                                  |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Sujeito                                                      |
| **Sinônimos**     | Empregado rural, Caseiro                                     |
| **Noção**         | [Funcionário](/docs/Product/Lexicons?id=funcionário) que trabalha na [fazenda](/docs/Product/Lexicons?id=fazenda), responsável por gerenciar o [gado](/docs/Product/Lexicons?id=bovino) e os [insumos](/docs/Product/Lexicons?id=insumo) |
| **Impacto**       | O [funcionário](/docs/Product/Lexicons?id=funcionário) poderá coletar dados dos [bovinos](/docs/Product/Lexicons?id=bovino)  <br />O [funcionário](/docs/Product/Lexicons?id=funcionário) poderá inserir informações sobre os [bovinos](/docs/Product/Lexicons?id=bovino) e os [insumos](/docs/Product/Lexicons?id=insumo) no aplicativo <br />Um [funcionário](/docs/Product/Lexicons?id=funcionário) pode cadastrar [bovinos](/docs/Product/Lexicons?id=bovino) e [insumos](/docs/Product/Lexicons?id=insumo) <br />Um [funcionário](/docs/Product/Lexicons?id=funcionário) pode editar seus dados, dados do [bovino](/docs/Product/Lexicons?id=bovino)  e do [insumo](/docs/Product/Lexicons?id=insumo)<br />Um [funcionário](/docs/Product/Lexicons?id=funcionário) pode gerar [relatórios](/docs/Product/Lexicons?id=relatório) referentes aos [bovinos](/docs/Product/Lexicons?id=bovino) |

### Proprietário
| **Nome**          | [Proprietário](/docs/Product/Lexicons?id=proprietário)                                                 |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Sujeito                                                      |
| **Sinônimos**     | Fazendeiro, Dono da [fazenda](/docs/Product/Lexicons?id=fazenda), Pecuarista, Produtos Rural                      |
| **Noção**         | Responsável por gerenciar a [fazenda](/docs/Product/Lexicons?id=fazenda)                          |
| **Impacto**       | [Proprietário](/docs/Product/Lexicons?id=proprietário) pode coletar dados dos [bovinos](/docs/Product/Lexicons?id=bovino) e dos [insumos](/docs/Product/Lexicons?id=insumo)<br />[Proprietário](/docs/Product/Lexicons?id=proprietário) pode inserir e remover esses dados no aplicativo <br />[Proprietário](/docs/Product/Lexicons?id=proprietário) pode visualizar seus gastos e ter um controle sobre eles <br />[Proprietário](/docs/Product/Lexicons?id=proprietário) pode editar seus dados, dados dos [bovinos](/docs/Product/Lexicons?id=bovino) e dos [insumos](/docs/Product/Lexicons?id=insumo) <br />[Proprietário](/docs/Product/Lexicons?id=proprietário) pode gerar [relatórios](/docs/Product/Lexicons?id=relatório) referentes aos [bovinos](/docs/Product/Lexicons?id=bovino) e aos seus gastos<br />[Proprietário](/docs/Product/Lexicons?id=proprietário) pode adicionar mais de uma [fazenda](/docs/Product/Lexicons?id=fazenda) |

### Relatório
| **Nome**          | Relatório                                                    |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Informações, Exposição de dados                              |
| **Noção**         | Conjunto de informações utilizado para reportar resultados coletados da [fazenda](/docs/Product/Lexicons?id=fazenda) |
| **Impacto**       | Gerar [relatórios](/docs/Product/Lexicons?id=relatório) sobre o estoque de alimentos, água, [vacinas](/docs/Product/Lexicons?id=vacina), etc... <br />Gerar [relatórios](/docs/Product/Lexicons?id=relatório) sobre os [bovinos](/docs/Product/Lexicons?id=bovino) <br />Gerar [relatórios](/docs/Product/Lexicons?id=relatório) sobre os gastos |

### Manejar
| **Nome**          | Manejar                        |
| ----------------- | ------------------------------ |
| **Classificação** | Verbo                          |
| **Sinônimos**     | Manipular o [gado](/docs/Product/Lexicons?id=bovino), Manusear. |
| **Noção**         | Transportar os [animais](/docs/Product/Lexicons?id=bovino)        |
| **Impacto**       | Gerar [relatórios](/docs/Product/Lexicons?id=relatório) a respeito dos vários tipos de [manejo](/docs/Product/Lexicons?id=manejar) realizados <br /> O [funcionário](/docs/Product/Lexicons?id=funcionário) e o [proprietário](/docs/Product/Lexicons?id=proprietário) são capazes de [manejar](/docs/Product/Lexicons?id=manejar) o [gado](/docs/Product/Lexicons?id=bovino) <br /> O [gado](/docs/Product/Lexicons?id=bovino) pode ser [manejado](/docs/Product/Lexicons?id=manejar)|

### Fazenda
| **Nome**          | Fazenda                                                      |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | [Propriedade rural](/docs/Product/Lexicons?id=proprietário), rancho, sítio                             |
| **Noção**         | [Propriedade rural](/docs/Product/Lexicons?id=proprietário) de lavoura ou de criação de gado           |
| **Impacto**       | Cadastrar uma [fazenda](/docs/Product/Lexicons?id=fazenda) <br />Editar os dados referentes a uma [fazenda](/docs/Product/Lexicons?id=fazenda) <br />Adicionar um [proprietário](/docs/Product/Lexicons?id=proprietário) para a [fazenda](/docs/Product/Lexicons?id=fazenda) |

<!-- Alterar -->
### Pasto 
| **Nome**          | Pasto                                                        |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Alimento [bovino](/docs/Product/Lexicons?id=bovino), ração                                       |
| **Noção**         | Vegetação utilizada para a alimentação do [gado](/docs/Product/Lexicons?id=bovino) e extensão ou terreno onde o [gado](/docs/Product/Lexicons?id=bovino) é deixado para se alimentar |
| **Impacto**       | Cadastrar uma [fazenda](/docs/Product/Lexicons?id=fazenda) <br />Editar os dados referentes a uma [fazenda](/docs/Product/Lexicons?id=fazenda) <br />Cadastrar um [bovino](/docs/Product/Lexicons?id=bovino) <br />Coletar dados do [bovino](/docs/Product/Lexicons?id=bovino) <br />Geração de [relatórios](/docs/Product/Lexicons?id=relatório) |

### GMD
| **Nome**          | GMD                                                          |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | [Ganho de Massa Diária](/docs/Product/Lexicons?id=gmd)                                        |
| **Noção**         | Índice referente ao ganho de massa diário de um [bovino](/docs/Product/Lexicons?id=bovino)       |
| **Impacto**       | A partir do [manejo](/docs/Product/Lexicons?id=manejar) de pesagem realizado no [bovino](/docs/Product/Lexicons?id=bovino) é possível calcular seu [Ganho de Massa Diário](/docs/Product/Lexicons?id=gmd) <br />[GMD](/docs/Product/Lexicons?id=gmd) é uma métrica para a geração de [relatórios](/docs/Product/Lexicons?id=relatório) <br /> O [proprietário](/docs/Product/Lexicons?id=proprietário) da [fazenda](/docs/Product/Lexicons?id=fazenda) pode optar por vender um [gado](/docs/Product/Lexicons?id=bovino) por conta do seu [GMD](/docs/Product/Lexicons?id=gmd) |

### RGD
| **Nome**          | RGD                                                          |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Registro genealógico definitivo                              |
| **Noção**         | Condição para que os filhos desse [gado](/docs/Product/Lexicons?id=bovino) não apresentem nenhuma desclassificação racial |
| **Impacto**       | [RGD](/docs/Product/Lexicons?id=rgd) é uma métrica para a geração de [relatórios](/docs/Product/Lexicons?id=relatório) <br />O [gado](/docs/Product/Lexicons?id=bovino) pode possuir o [RGD](/docs/Product/Lexicons?id=rgd) ao ser cadastrado no aplicativo <br />O [fazendeiro](/docs/Product/Lexicons?id=proprietário) pode deixar de comprar um [gado](/docs/Product/Lexicons?id=bovino) por ele não possuir [RGD](/docs/Product/Lexicons?id=rgd) <br />O [Registro genealógico definitivo](/docs/Product/Lexicons?id=rgd) do [gado](/docs/Product/Lexicons?id=bovino) pode ser adicionado após seu cadastro no aplicativo|

### Hectare
| **Nome**          | Hectare                                                      |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Área, unidade de medida                                      |
| **Noção**         | Unidade de medida de área equivalente a 100 ares ou a 10 000 metros quadrados |
| **Impacto**       | Ao cadastrar uma [fazenda](/docs/Product/Lexicons?id=fazenda) é necessário informar quantos [Hectares](/docs/Product/Lexicons?id=hectare) ela possui<br />A geração de [relatórios](/docs/Product/Lexicons?id=relatório) considera a [área](/docs/Product/Lexicons?id=hectare) da [fazenda](/docs/Product/Lexicons?id=fazenda) nos cálculos <br />Lucro Por [Hectare](/docs/Product/Lexicons?id=hectare) Por Ano |

### Taxa de Lotação
| **Nome**          | Taxa de Lotação                                              |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | -                                                             |
| **Noção**         | A [taxa de lotação](/docs/Product/Lexicons?id=taxa-de-lotação) é definida pelo número de animais dividido pela área do [pasto](/docs/Product/Lexicons?id=pasto) |
| **Impacto**       | A [taxa de lotação](/docs/Product/Lexicons?id=taxa-de-lotação) depende da [fazenda](/docs/Product/Lexicons?id=fazenda) para ser calculada <br />Cadastrar [gado](/docs/Product/Lexicons?id=bovino) altera o valor da [taxa de lotação](/docs/Product/Lexicons?id=taxa-de-lotação) <br />Geração de [relatórios](/docs/Product/Lexicons?id=relatório) utiliza a [taxa de lotação](/docs/Product/Lexicons?id=taxa-de-lotação) como um dos dados |

### Prenhez
| **Nome**          | Prenhez                                                      |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Estado                                                       |
| **Sinônimos**     | Gravidez, fetação, gestação                                  |
| **Noção**         | Estado em que a [vaca](/docs/Product/Lexicons?id=bovino) está prenha                             |
| **Impacto**       | Adicionar esse dado como verdadeiro se a [vaca](/docs/Product/Lexicons?id=bovino) estiver [prenha](/docs/Product/Lexicons?id=prenhez) <br /> O [proprietário](/docs/Product/Lexicons?id=proprietário) pode saber se a vaca está [prenha](/docs/Product/Lexicons?id=prenhez) ou não <br />A [prenhez](/docs/Product/Lexicons?id=prenhez) pode trazer um custo benefício vantajoso ao [produtor rural](/docs/Product/Lexicons?id=proprietário) |

### Gado de Corte 
| **Nome**          | Gado de Corte                                                |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Pecuária de corte                                            |
| **Noção**         | O [gado](/docs/Product/Lexicons?id=bovino) de corte é o [gado](/docs/Product/Lexicons?id=bovino) criado para a produção de carne    |
| **Impacto**       | Adicionar [gado](/docs/Product/Lexicons?id=bovino) de corte para obter metricas na geracão de [relatórios](/docs/Product/Lexicons?id=relatório) e lucros |

### Gado de Leite 
| **Nome**          | Gado de Leite                                                |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Pecuária de leite                                            |
| **Noção**         | O [gado](/docs/Product/Lexicons?id=bovino) de leite é o [gado](/docs/Product/Lexicons?id=bovino) criado para a produção de leite    |
| **Impacto**       | Adicionar [gado](/docs/Product/Lexicons?id=bovino) de leite para obter métricas na geração de [relatórios](/docs/Product/Lexicons?id=relatório) e lucros com a venda de produtos lácteos <br />O [gado de leite](/docs/Product/Lexicons?id=gado-de-leite) pode entrar em estado de [prenhez](/docs/Product/Lexicons?id=prenhez) após sofrer um [manejo](/docs/Product/Lexicons?id=manejar) de reprodução|

### Taxa de Desmama   
| **Nome**          | Taxa de Desmama                                              |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | -                                                            |
| **Noção**         | Representa o total de [bovinos](/docs/Product/Lexicons?id=bovino) desmamados em relação às [vacas](/docs/Product/Lexicons?id=bovino) expostas em reprodução dentro de um determinado período |
| **Impacto**       | A geração de [relatórios](/docs/Product/Lexicons?id=relatório) utilizará a [Taxa de Desmama](/docs/Product/Lexicons?id=taxa-de-desmama) como um dos dados para cálculo|

### Insumo
| **Nome**          | Insumo                                                       |
| ----------------- | ------------------------------------------------------------ |
| **Classificação** | Objeto                                                       |
| **Sinônimos**     | Matéria-prima, Material                                      |
| **Noção**         | Os insumos pecuários compreendem os produtos de uso veterinário, os produtos destinados à alimentação [animal](/docs/Product/Lexicons?id=bovino), o material genético [animal](/docs/Product/Lexicons?id=bovino) e do registro genealógico dos [animais](/docs/Product/Lexicons?id=bovino) |
| **Impacto**       | O [fazendeiro](/docs/Product/Lexicons?id=proprietário) e o [funcionário](/docs/Product/Lexicons?id=funcionário) podem adicionar novos [insumos](/docs/Product/Lexicons?id=insumo), editar os [insumos](/docs/Product/Lexicons?id=insumo) já cadastrados ou apagá-los|

## Referências
* Julio Leite. A Strategy for Conceptual Model Acquisition. IEEE 1992.
* Requisitos de Software - Wire, Léxicos. Disponível em: <https://requisitos-de-software.github.io/2019.2-Wire/#/docs/modeling/lexicons>