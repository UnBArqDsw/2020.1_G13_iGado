# Padrões de Projeto Emergentes

|    Data    | Versão |         Descrição         |           Autor(es)           |
| :--------: | :----: | :-----------------------: | :---------------------------: |
| 07/10/2020 |  0.1   | Definições iniciais e referências | [Iuri Severo](https://github.com/iurisevero) |
| 07/10/2020 |  0.2   | Adição do padrão Singleton | [Iuri Severo](https://github.com/iurisevero) |

<p align="justify"> &emsp;&emsp; Padrões de projetos são pricípior e soluções adotadas para resolver problemas comuns encontrados durante o desenvolvimento de um projeto de software. Esse padrões são documentados e visam seguir uma estrutura e um comportamento regular para solucionar um problema específico a partir de sua aplicação. <br />
&emsp;&emsp; No entanto, fatores como: <i>(i)</i> falta de conhecimento da implementação do padrão por parte do desenvolvedor; <i>(ii)</i> sucessivas mudanças em outras classes e refletidas nessa parte do código; <i>(iii)</i> falta de refatoração no código; ou, <i>(iv)</i> característica do problema e não necessita implementar o padrão <i>(Job, 2014, p. 27)</i>, podem resultar em situações onde se tem um padrão comportamental não estruturado, aspecto comum de padrões emergentes. <br />

## Singleton

<p align="justify"> &emsp;&emsp; O Singleton é um padrão adotado para classes que só podem possuir uma instância no projeto. Por exemplo, a classe que vai guardar os dados do jogador em um jogo. A ideia base é tornar o construtor do objeto privado, para que ninguém além da própria classe possa criar uma instância dele (Loviscach, 2012). Em vez disso, a classe fornece um método estático do qual é possível obter a instância já existente. </p>

_Figura 1.1: Padrão Singleton_
<br /><img src="docs/Assets/Img/Studies/EmergingDesignPatterns/SingletonPattern.png" alt="Padrão Singleton"><br />
_Fonte: Job, 2014, p.2_

_Código Fonte 1.1: O Padrão Singleton na classe Licences_
```
// Os imports , atributo s e demais métodos foram omitido s
public class Licences {
    public static final String GPL = "GNU LICENSE";
    public static final String LGPL = "GNU LESSER PUBLIC LICENSE";
    /** Um atributo privado e estático. */
    private static Licences singleton ;
    /** Returna uma referencia desta classe. */
    public static Licences getlnstance() {
        if (singleton == null ) {
            singleton = new Licences() ;
        }
        return singleton ;
    }
    public String getGPL() {
        return GPL;
    }
    public String getLGPL() {
        return LGPL;
    }
}
```
_Fonte: Job, 2014, p.28~29_

## Referências
* JOB, Ricardo de Sousa. Uma abordagem para detecção de padrões emergentes. Disponível em: <http://dspace.sti.ufcg.edu.br:8080/jspui/handle/riufcg/944>. Acessado em setembro de 2020.
* SERRANO, Milene. Arquitetura e Desenho de Software AULA - GRASP – PARTE I. Acessado em setembro de 2020.
* LOVISCACH, Jörn. Design Patterns. Events. Disponível em: <https://doi.org/10.5446/9689>. Acessado em setembro de 2020.