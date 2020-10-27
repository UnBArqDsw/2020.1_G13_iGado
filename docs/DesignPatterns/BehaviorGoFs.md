# Aplicação de GoF(s) Comportamentais

|    Data    | Versão |                Descrição                |                     Autor(es)                     |
| :--------: | :----: | :-------------------------------------: | :-------------------------------------------: |
| 25/10/2020 | 0.1 | Criação do Documento da aplicação dos GoFs Comportamentais | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 25/10/2020 | 0.2 | Adição do padrão <i>Iterator</i> | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 25/10/2020 | 0.3 | Adição do padrão <i>Memento</i> | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 25/10/2020 | 0.4 | Adição do padrão <i>Template Method</i> | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 25/10/2020 | 0.5 | Adição do padrão <i>State</i> | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 26/10/2020 | 1.0 | Revisão do documento | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |

## Iterator

<p align="justify"> &emsp;&emsp; A aplicação deste padrão é dada no ato de percorrer listas para trazer todos os usuários cadastrados no banco de dados. </p>

<img src="docs/Assets/Img/DesignPatterns/BehaviorGoFs/IteratorExample.png" alt="Iterator Example">

[project/api/resources/user.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/blob/master/project/api/resources/user.py) <br />
[project/api/models/user.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/blob/master/project/api/models/user.py)

## Memento

<p align="justify"> &emsp;&emsp; O Flutter usa o padrão memento na pilha de navegação. </p>

<img src="docs/Assets/Img/DesignPatterns/BehaviorGoFs/MementoExample.jpg" alt="Memento Example">

[lib/screens/register_screen.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/blob/master/lib/screens/register_screen.dart)

## Template Method

<p align="justify"> &emsp;&emsp; O Template Method foi utilizado para gerar um padrão na criação dos relatórios. </p>

<img src="docs/Assets/Img/DesignPatterns/BehaviorGoFs/TemplateMethodExample.jpg" alt="Template Method Example"> <br />

<img src="docs/Assets/Img/DesignPatterns/BehaviorGoFs/TemplateMethodExample2.png" alt="Template Method Example 2"> <br />

<img src="docs/Assets/Img/DesignPatterns/BehaviorGoFs/TemplateMethodExample3.png" alt="Template Method Example 3"> <br />

[project/api/models/report.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/blob/113-DesignPatnersReport/project/api/models/report.py) <br />
[project/api/models/general_report.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/blob/113-DesignPatnersReport/project/api/models/general_report.py) <br />
[project/api/models/gmd_report.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/blob/113-DesignPatnersReport/project/api/models/gmd_report.py)

## State

<p align="justify"> &emsp;&emsp; O State foi utilizado para </p>
<img src="docs/Assets/Img/DesignPatterns/BehaviorGoFs/StateExample.png" alt="State Example"> <br />

[master/lib/screens/register_screen.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/blob/master/lib/screens/register_screen.dart) <br />
[master/lib/screens/login_screen.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/blob/master/lib/screens/login_screen.dart)

# Referências

* PAX - Dinâmica e Seminário 4. Disponível em <https://pax-app.github.io/Wiki/#/docs/DS/dinamica-e-seminario-4-b/README>. Acessado em: 25 de outubro de 2020.