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

Caso não seja utilizado o script, deve-se seguir esses passos:

* Os _commits_ devem ser escritos em inglês, na forma infinitiva, e ainda conter uma breve descrição:

**Exemplo:**

```Create a new document```

* A *issue* deve ser citada no commit por questões de rastreabilidade, para isso, basta adicionar:

```
#<number_of_issue>
```

**Exemplo:**

```#01 Create a new document```

**Observação:** Por padrão, o caracter '#' define uma linha de comentário na mensagem do *commit*. Para resolver esse problema, digite na linha de comando:

```git config --local core.commentChar '!'```

* Para que uma pessoa seja inclusa como contribuinte no gráfico de *commits* do GitHub, basta incluir a instrução ```Co-authored-By:``` na mensagem:

**Exemplo:**

```
#01 Create a new document


Co-authored-By: Lucas Fellipe <lucasfcm9@gmail.com>
Co-authored-By: Guilherme Mendes <guimendesp12@gmail.com>
```

* Para _commits_ que encerram a resolução de uma _issue_, deve-se iniciar a mensagem do _commit_ com Fix ```#<numero_da_issue> <mensagem>```, para que a _issue_ seja encerrada automaticamente quando mesclada na ```master```.

**Exemplo:**

```
Fix #5 Create a new document.
```

* Para _commits_ que incluem uma pequena mudança em uma _issue_ que já teve sua resolução encerrada, deve-se iniciar a mensagem do _commit_ com HOTFIX ```#<numero_da_issue> <mensagem>```

**Exemplo:**

```
HOTFIX #5 Add new anwser
```

