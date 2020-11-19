# Reutilização de Software

|    Data    | Versão |                Descrição                |                     Autor(es)                     |
| :--------: | :----: | :-------------------------------------: | :-------------------------------------------: |
| 17/11/2020 | 0.1 | Criação da estrutura inicial do documento | [Iuri Severo](https://github.com/iurisevero) |
| 17/11/2020 | 0.2 | Adição de informações sobre o framework Flutter | [Iuri Severo](https://github.com/iurisevero) |
| 17/11/2020 | 0.3 | Adição de informações sobre o microframework Flask | [Iuri Severo](https://github.com/iurisevero) |
| 17/11/2020 | 0.4 | Adição de informações sobre as bibliotecas utilizadas no Frontend | [Iuri Severo](https://github.com/iurisevero) |
| 17/11/2020 | 0.5 | Adição de informações sobre os plugins utilizados no Backend | [Iuri Severo](https://github.com/iurisevero) |
| 18/11/2020 | 0.6 | Adição de informações sobre as bibliotecas do backend e unittest | [Iuri Severo](https://github.com/iurisevero) |
| 18/11/2020 | 0.7 | Adição de informações sobre os widgets personalizados e formatação do arquivo e das referências | [Iuri Severo](https://github.com/iurisevero) |

## Frameworks

### Flask

<p align="justify"> &emsp;&emsp; Flask é um microframework de python baseado em Werkzeug, Jinja 2 e good intentions, que tem como objetivo ser uma base para o desenvolvimento de diversas aplicações. Para isso, ele possui um _core_ simples, porém extensível, que permite os desenvolvedores realizarem seus objetivos por conta própria ou pelo uso dos diversos pacotes e bibliotecas existentes para o framework. </p>

### Unittest

<p align="justify"> &emsp;&emsp; A estrutura de testes unitários unittest foi originalmente inspirada por JUnit e tem um comportamento semelhante aos principais frameworks de testes unitários em outras linguagens. Ele suporta automação de teste, compartilhamento de configuração e código de desligamento para testes, agregação de testes em coleções e independência dos testes da estrutura de relatório. </p>

### Flutter

<p align="justify"> &emsp;&emsp; Flutter é um conjunto de ferramentas que facilitam o desenvolvimento de interfaces de tamanhos variados e para todos tipos de aparelho. O framework trabalha principalmente a partir de Widgets que, por meio de um relacionamento de composição, permitem ao desenvolvedor utilizar diversos elementos de UI pré definidos. Além disso, o framework também permite ao usuário criar Widgets próprios e páginas por meio da herança de objetos abstratos como o ```StatefulWidget```. </p>

<img src="docs/Assets/Img/Project/SoftwareReuse/StatefulWidget.png"> <br />
Código retirado de: <https://github.com/flutter/flutter/blob/master/packages/flutter/lib/src/widgets/framework.dart>

## Bibliotecas

### Bibliotecas utilizadas no Backend

**sys**: Este módulo fornece acesso a algumas variáveis usadas ou mantidas pelo interpretador e a funções que interagem fortemente com o interpretador; <br />
**abc**: Este módulo fornece a infraestrutura para definir classes básicas abstratas (ABCs) em Python; <br />
**os**: Este módulo fornece uma maneira portátil de usar a funcionalidades dependentes do sistema operacional.

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
**Flask-JWT-Extended**: Flask-JWT-Extended adiciona suporte para o uso de [JSON Web Tokens (JWT)](https://jwt.io/) ao Flask para proteção de visualizações e também muitos recursos úteis (e opcionais) integrados para facilitar o trabalho com JSON Web Tokens; <br />
**flask-bcrypt**: Flask-Bcrypt é uma extensão do Flask que fornece utilitários de hash bcrypt para a aplicação desenvolvida; <br />
**psycopg2-binary**: Psycopg é o adaptador de banco de dados PostgreSQL mais popular para a linguagem de programação Python. Suas principais características são a implementação completa da especificação Python DB API 2.0 e a segurança de thread.

## Serviços

### Gunicorn

<p align="justify"> &emsp;&emsp; Gunicorn 'Green Unicorn' é um servidor Python WSGI HTTP para UNIX. É um modelo de trabalhador pre-fork. O servidor Gunicorn é amplamente compatível com vários frameworks da web, simplesmente implementado, com recursos de servidor leves e bastante rápido. </p>

## Outros

### Widgets Personalizados

<p align="justify"> &emsp;&emsp; Uma das funcionalidades disponibilizadas pelo Flutter é a de criar _Widgets_ personalizados melhorar a reutilização de código. Essa prática também é adotada em outros frameworks voltados para desenvolvimento UI como os _components_ do React Native. </p>

No projeto iGado os _Widgets_ personalizados podem ser encontrado na pasta [2020.1_G13_iGado_Frontend/lib/components](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/tree/master/lib/components). Os _Widgets_ criados pelo grupo foram:

* [dropdown_icon_text.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/blob/master/lib/components/dropdown_icon_text.dart)
* [icon_text_form_field.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/blob/master/lib/components/icon_text_form_field.dart)
* [radio_button_transform.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/blob/master/lib/components/radio_button_transform.dart)
* [simple_card.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/blob/master/lib/components/simple_card.dart)
* [title_text_form_field.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/blob/master/lib/components/title_text_form_field.dart)
* [visibility_form_field.dart](https://github.com/UnBArqDsw/2020.1_G13_iGado_Frontend/blob/master/lib/components/visibility_form_field.dart)

## Referências

* Flutter architectural overview. Disponível em: <https://flutter.dev/docs/resources/architectural-overview>. Acessado em Novembro de 2020;
* Flutter - Using packages. Disponível em: <https://flutter.dev/docs/development/packages-and-plugins/using-packages>. Acessado em Novembro de 2020;
* Flutter API reference documentation. Disponível em: <https://api.flutter.dev/flutter>. Acessado em Novembro de 2020;
* RFlutter Alert. Disponível em: <https://pub.dev/packages/rflutter_alert>. Acessado em Novembro de 2020;
* Design Decisions in Flask. Disponível em: <https://flask.palletsprojects.com/en/1.1.x/design/>. Acessado em Novembro de 2020;
* Flask - Foreword. Disponível em: <https://flask.palletsprojects.com/en/1.1.x/foreword/>. Acessado em Novembro de 2020;
* Flask-RESTful. Disponível em: <https://flask-restful.readthedocs.io/en/latest/>. Acessado em Novembro de 2020;
* Flask-SQLAlchemy. Disponível em: <https://flask-sqlalchemy.palletsprojects.com/en/2.x/>. Acessado em Novembro de 2020;
* Flask-Testing. Disponível em: <https://pythonhosted.org/Flask-Testing/>. Acessado em Novembro de 2020;
* Flask-JWT-Extended. Disponível em: <https://pypi.org/project/Flask-JWT-Extended/>. Acessado em Novembro de 2020;
* Flask-Bcrypt. Disponível em: <https://flask-bcrypt.readthedocs.io/en/latest/>. Acessado em Novembro de 2020;
* Gunicorn. Disponível em: <https://gunicorn.org/>. Acessado em Novembro de 2020;
* Psycopg2-binary. Disponível em: <https://pypi.org/project/psycopg2-binary/>. Acessado em Novembro de 2020;
* Unittest — Unit testing framework. Disponível em: <https://docs.python.org/3/library/unittest.html?highlight=unittest#module-unittest>. Acessado em Novembro de 2020;
