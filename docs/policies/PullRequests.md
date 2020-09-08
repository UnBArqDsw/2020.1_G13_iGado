# Política de Pull Requests

| Data       | Versão | Descrição            | Autor             |
|:----------:|:------:|:--------------------:|:-----------------:|
| 25/08/2020 | 0.1 | Criação do documento com template inicial  | Lucas Fellipe, Iuri Severo, Guilherme Mendes, Caio Vinicius e João Pedro |

Os _pull requests_ devem seguir o seguinte padrão:

* O _pull request_ deve indicar em seu título o número e nome da _issue_, ao qual _issue_ se refere.

<b>Exemplo</b>

```
#1 Criação da Rich Picture
```

* Para indicar que o _pull request_ ainda não está completo para o merge, usa-se a 'tag' WIP(_Work in Progress_).

<b>Exemplo</b>

```
WIP #1 NovoDocumento
```

* Para o conteúdo do _pull request_, deve ser descrito de forma sucinta.

```
Neste pull request se realizou:
  * US 01
  * Validação
  * Testes
  * Correção de bug ao...
```

* Deve conter um ```Reviewer```, em que indica-se pelo menos um membro da equipe de Arquitetura & Desenho de Software a ser responsável por analisar as modificações submetidas.

* Deve conter um ou mais ```Assignees```, em que indica os membros da equipe que contribuíram com as modificações realizadas.

* Deve conter ```Labels```, em que adicionam-se as labels referentes ao _pull request_, de forma similar às da _issue_ correspondente.

* Deve conter a ```Milestone```, em que é adicionada a sprint correspondente à execução das modificações.

* Deve conter a ```Issue```, em que, após a criação do _pull request_, deve-se conectar ele à sua _issue_ correspondente através da interface do Github.
