# Política de Branches

| Data       | Versão | Descrição            | Autor             |
|:----------:|:------:|:--------------------:|:-----------------:|
| 25/08/2020 | 0.1 | Criação do documento com template inicial  | Lucas Fellipe, Iuri Severo, Guilherme Mendes, Caio Vinicius e João Pedro |

As _branches_ devem seguir o seguinte padrão:

* O nome da branch deve ser abstraído do nome da história de usuário a qual se refere.

<b>Exemplo:</b>

```
CriarLogin
```

* O nome da _branch_ deve possuir um 'tag' que é o número da história de usuário a qual se refere.

<b>Exemplo:</b>

```
3CriarLogin
```

* A _branch_ deverá possuir o padrão CamelCase ```x-NomeDaBranch ```, em que o 'x' é o número da história de usuário.

<b>Exemplo:</b>

```
3-CriarLogin
```

* Caso a _branch_ não esteja associada a alguma história de usuário, não é necessario a adição da 'tag'.

<b>Exemplo:</b>

```
RefatorarLogin
```
