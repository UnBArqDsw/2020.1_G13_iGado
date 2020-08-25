# Política de Commits

| Data       | Versão | Descrição            | Autor             |
|:----------:|:------:|:--------------------:|:-----------------:|
| 25/08/2020 | 0.1 | Criação do documento com template inicial  | Lucas Fellipe, Iuri Severo, Guilherme Mendes, Caio Vinicius e João Pedro |

 Os _commits_ devem ser realizados usando um script de _commit_ disponibilizado na pasta raiz do repositório da disciplina de Arquitetura & Desenho de Software.

Para disponibilizá-lo como um comando nativo do terminal, basta digitar no terminal:

```chmod u+x commit```

E para que o comando de _commit_ seja executado, basta digitar:
```
./commit <mensagem de commit>
```

Logo após digitar o comando ```./commit <mensagem de commit>```, basta seguir o passo-a-passo do que o script pede.

* Os _commits_ devem ser escritos em inglês na forma infinitiva, e ainda conter uma breve decrição.

<b>Exemplo: <b>

```
Create a new document.
```

* A issue em questão deve ser citada no _commit_, para isso, basta adicionar 
``` #<numero_da_issue>. ```

<b>Exemplo: <b>

```
#5 Create a new document.
```

* Para _commits_ que encerram a resolução de uma _issue_, deve-se iniciar a mensagem do _commit_ com Fix ```#<numero_da_issue> <mensagem>```, para que a _issue_ seja encerrada automaticamente quando mesclada na ```master```.

<b>Exemplo: <b>

```
Fix #5 Create a new document.
```

* Para _commits_ que incluem uma pequena mudança em uma _issue_ que já teve sua resolução encerrada, deve-se iniciar a mensagem do _commit_ com HOTFIX ```#<numero_da_issue> <mensagem>```

<b>Exemplo: <b>

```
HOTFIX #5 Add new anwser.
```
