# Reutilização de Software

|    Data    | Versão |                Descrição                |                     Autor(es)                     |
| :--------: | :----: | :-------------------------------------: | :-------------------------------------------: |
| 17/11/2020 | 0.1 | Criação da estrutura inicial do documento | [Iuri Severo](https://github.com/iurisevero) |
| 17/11/2020 | 0.2 | Adição de informações sobre o framework Flutter | [Iuri Severo](https://github.com/iurisevero) |
| 17/11/2020 | 0.3 | Adição de informações sobre o microframework Flask | [Iuri Severo](https://github.com/iurisevero) |
| 17/11/2020 | 0.4 | Adição de informações sobre as bibliotecas utilizadas no Frontend | [Iuri Severo](https://github.com/iurisevero) |
| 17/11/2020 | 0.5 | Adição de informações sobre os plugins utilizados no Backend | [Iuri Severo](https://github.com/iurisevero) |

## Frameworks

### Flask

Flask é um microframework de python baseado em Werkzeug, Jinja 2 e good intentions, que tem como objetivo ser uma base para o desenvolvimento de diversas aplicações. Para isso, ele possui um _core_ simples, porém extensível, que permite os desenvolvedores realizarem seus objetivos por conta própria ou pelo uso dos diversos pacotes e bibliotecas existentes para o framework.

### Flutter

Flutter é um conjunto de ferramentas que facilitam o desenvolvimento de interfaces de tamanhos variados e para todos tipos de aparelho. O framework trabalha principalmente a partir de Widgets que, por meio de um relacionamento de composição, permitem ao desenvolvedor utilizar diversos elementos de UI pré definidos. Além disso, o framework também permite ao usuário criar Widgets próprios e páginas por meio da herança de objetos abstratos como o ```StatefulWidget```.

<img src="docs/Assets/Img/Project/SoftwareReuse/StatefulWidget.png"> <br />
Código retirado de: <https://github.com/flutter/flutter/blob/master/packages/flutter/lib/src/widgets/framework.dart>

## Bibliotecas

### Bibliotecas utilizadas no Backend



### Bibliotecas utilizadas no Frontend

**flutter/material.dart**: Biblioteca que permite os _widgets_ do Flutter implementarem _[Material Desing](https://material.io/design)_; <br />
**flutter/widgets.dart**: Estrutura de _widgets_ do Flutter; <br />
**rflutter_alert/rflutter_alert.dart**: Biblioteca para criação de alertas e _popups_ customizáveis; <br />
**flutter_test/flutter_test.dart**: Biblioteca de testes para flutter, criada a partir do pacote _[test](https://pub.dev/packages/test)_;

## Plugins

### Plugins utilizados no Backend

**Flask-RESTful**: Flask-RESTful é uma extensão para Flask que adiciona suporte para a criação rápida de APIs REST. Ela é uma leve abstração que trabalha com as bibliotecas/ORM existentes; <br />
**Flask-SQLAlchemy**: Flask-SQLAlchemy é uma extensão do Flask que adiciona suporte para SQLAlchemy ao aplicativo desenvolvido. Ela visa simplificar o uso do SQLAlchemy com o Flask, fornecendo padrões úteis e auxiliares extras que tornam mais fácil a realização de tarefas comuns; <br />
**Flask-Testing**: A extensão Flask-Testing fornece utilitários de testes unitários para Flask; <br />
**Flask-JWT**: Adicione recursos [JWT](https://jwt.io/) básicos ao seu aplicativo Flask; <br />
**Flask-JWT-Extended**: Flask-JWT-Extended adiciona suporte para o uso de [JSON Web Tokens (JWT)](https://jwt.io/) ao Flask para proteção de visualizações e também muitos recursos úteis (e opcionais) integrados para facilitar o trabalho com JSON Web Tokens; <br />
**flask-bcrypt**: Flask-Bcrypt é uma extensão do Flask que fornece utilitários de hash bcrypt para a aplicação desenvolvida;
<!-- **psycopg2-binary**: <br /> conferir se é um plugin -->
<!-- **gunicorn**: <br /> conferir se é um plugin -->

## Serviços

### iGado Server
* Caixa preta
    * Por consumo de programação pronta
* de Integração

## Referências

* <https://flutter.dev/docs/resources/architectural-overview>
* <https://flutter.dev/docs/development/packages-and-plugins/using-packages>
* <https://api.flutter.dev/flutter>
* <https://pub.dev/packages/rflutter_alert>
* <https://flask.palletsprojects.com/en/1.1.x/design/>
* <https://flask.palletsprojects.com/en/1.1.x/foreword/>
* <https://flask-restful.readthedocs.io/en/latest/>
* <https://flask-sqlalchemy.palletsprojects.com/en/2.x/>
* <https://pythonhosted.org/Flask-Testing/>
* <https://pythonhosted.org/Flask-JWT/>
* <https://pypi.org/project/Flask-JWT-Extended/>
* <https://flask-bcrypt.readthedocs.io/en/latest/>
