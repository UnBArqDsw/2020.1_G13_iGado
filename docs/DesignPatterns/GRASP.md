# Aplicação de GRASP(s)

|    Data    | Versão |                Descrição                |                     Autor(es)                     |
| :--------: | :----: | :-------------------------------------: | :-------------------------------------------: |
| 25/10/2020 | 0.1 | Criação do Documento da aplicação dos GRASP(s) | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 25/10/2020 | 0.2 | Adição do GRASP <i>Polimorfismo</i> | [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |
| 26/10/2020 | 0.3 | Adição dos GRASP's  Criador, Especialista, Coesão, Invenção Própria, Controller| [Caio Vinícius](https://github.com/caiovfernandes), [Guilherme Mendes](https://github.com/guilherme-mendes), [Iuri Severo](https://github.com/iurisevero), [João Guedes](https://github.com/sudjoao) e [Lucas Fellipe](https://github.com/lucasfcm9) |

## Polimorfismo
<img src="docs/Assets/Img/DesignPatterns/GRAPS/BovinePolimorfism.png"><br/>

[project/api/models/bovine.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/tree/master/project/api/models/bovine.py) <br/>

<img src="docs/Assets/Img/DesignPatterns/GRAPS/DairyCattle.png"> <br/>

[project/api/models/dairy_cattle.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/tree/master/project/api/models/dairy_cattle.py)

<img src="docs/Assets/Img/DesignPatterns/GRAPS/PolimorfismExample.png" alt="Polimorfism Example">

[Class Diagram](https://unbarqdsw.github.io/2020.1_G13_iGado/#/docs/Modeling/ClassDiagram) <br />

## Criador
<img src="docs/Assets/Img/DesignPatterns/GRAPS/ReportPolimorfism.png">

[project/api/generator_report/generator_report.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/tree/master/project/api/generator_report/generator_report.py) <br />
[project/api/models/user.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/tree/master/project/api/models/user.py) <br />

## Especialista
<img src="docs/Assets/Img/DesignPatterns/GRAPS/EspecialistService.png">

[lib/services/api.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/tree/master/lib/services/api.dart) <br/>
[lib/services/login_service.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/tree/master/lib/services/login_service.dart)<br/>
[lib/services/user_service.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/tree/master/lib/services/user_service.dart)

## Coesão
<img src="docs/Assets/Img/DesignPatterns/GRAPS/CohesionModelFarm.png">

[project/api/models/farm.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/tree/master/project/api/models/farm.py)<br/>
[project/api/models/general_report.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/tree/master/project/api/models/general_report.py)<br/>
[project/api/models/gmd_report.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/tree/master/project/api/models/gmd_report.py)<br/>
[project/api/models/report.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/tree/master/project/api/models/report.py)<br/>
[project/api/models/user.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/tree/master/project/api/models/user.py)<br/>
[project/api/models/work.py](https://github.com/UnBArqDsw/2020.1_G13_iGado_Backend/tree/master/project/api/models/work.py)<br/>

## Invenção Própria
<img src="docs/Assets/Img/DesignPatterns/GRAPS/OwnInvestmentServices.png">

[lib/services/api.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/tree/master/lib/services/api.dart) <br/>
[lib/services/login_service.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/tree/master/lib/services/login_service.dart)<br/>
[lib/services/user_service.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/tree/master/lib/services/user_service.dart)

## Controller
<img src="docs/Assets/Img/DesignPatterns/GRAPS/ControllerServices.png">

[lib/services/api.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/tree/master/lib/services/api.dart) <br/>
[lib/services/login_service.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/tree/master/lib/services/login_service.dart)<br/>
[lib/services/user_service.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/tree/master/lib/services/user_service.dart)

# Referências

* PAX - Dinâmica e Seminário 4. Disponível em <https://pax-app.github.io/Wiki/#/docs/DS/dinamica-e-seminario-4-b/README>. Acessado em: 25 de outubro de 2020.