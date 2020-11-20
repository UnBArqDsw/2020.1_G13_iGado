# Padrões de Projeto Emergentes

|    Data    | Versão |         Descrição         |           Autor(es)           |
| :--------: | :----: | :-----------------------: | :---------------------------: |
| 07/10/2020 |  0.1   | Definições iniciais e referências | [Iuri Severo](https://github.com/iurisevero) |
| 07/10/2020 |  0.2   | Adição do padrão Singleton | [Iuri Severo](https://github.com/iurisevero) |
| 07/10/2020 |  0.3   | Adição do padrão Composite | [Iuri Severo](https://github.com/iurisevero) |
| 07/10/2020 |  0.4   | Adição do padrão State e Factory Method | [Iuri Severo](https://github.com/iurisevero) |
| 10/10/2020 |  1.0   | Revisão do estudo de Padroões de Projeto Emergentes | [Guilherme Mendes](https://github.com/guilherme-mendes) |
| 26/10/2020 | 1.1 | Adição do vídeo de apresentação dos padrões para o grupo | [João Pedro Guedes](https://github.com/sudjoao)|

## Introdução

<p align="justify"> &emsp;&emsp; Padrões de projetos são pricípios e soluções adotadas para resolver problemas comuns encontrados durante o desenvolvimento de um projeto de software. Esse padrões são documentados e visam seguir uma estrutura e um comportamento regular para solucionar um problema específico a partir de sua aplicação. <br />
&emsp;&emsp; No entanto, fatores como: <i>(i)</i> falta de conhecimento da implementação do padrão por parte do desenvolvedor; <i>(ii)</i> sucessivas mudanças em outras classes e refletidas nessa parte do código; <i>(iii)</i> falta de refatoração no código; ou, <i>(iv)</i> característica do problema e não necessita implementar o padrão <i>(Job, 2014, p. 27)</i>, podem resultar em situações onde se tem um padrão comportamental não estruturado, aspecto comum de padrões emergentes. <br />

<a href="https://www.youtube.com/watch?v=_3oL4v1HCIc&feature=youtu.be">Vídeo de Apresentação dos Padrões para o grupo</a>

## Singleton

<p align="justify"> &emsp;&emsp; O Singleton é um padrão adotado para classes que só podem possuir uma instância no projeto. Por exemplo, a classe que vai guardar os dados do jogador em um jogo. A ideia base é tornar o construtor do objeto privado, para que ninguém além da própria classe possa criar uma instância dele (Loviscach, 2012). Em vez disso, a classe fornece um método estático do qual é possível obter a instância já existente. </p>

_Figura 1.1: Padrão Singleton_
<br /><img src="docs/Assets/Img/Studies/EmergingDesignPatterns/SingletonPattern.png" alt="Padrão Singleton"><br />
_Fonte: Job, 2014, p.2_

_Código Fonte 1.1: O padrão Singleton em estado emergente na classe Licences_
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

<p align="justify"> &emsp;&emsp;  No código acima é possível ver os padrões estruturais do Singleton, exceto pelo construtor da classe <code>Licence</code> que não é especificado. Isso a faz ser classificada como um padrão emergente, visto que não segue a risca os padrões de projeto. </p>

## Composite

<p align="justify"> &emsp;&emsp; O padrão <b>Composite</b> é adotado quando é necessário tratar um conjunto de objetos como uma singularidade. Um exemplo dessa ação pode ser encontrado em diversos softwares de edição de imagem e desenho, na função de agrupamento: diversos objetos distintos passam a ser tratados como um só, o grupo, o qual é possível movimentar, redimensionar, duplicar, etc..</p>
<p align="justify"> &emsp;&emsp; A solução adotada para isso é uma hierarquia de classes baseada em dois objetos, um <i>Composite Object</i> e uma <i>Leaf Object</i>, onde o <i>Composite Object</i> é uma combinação de elementos individuais e outros <i>Composites Objects</i>, e a <i>Leaf Object</i> é o objeto individual. O resultado disso é uma estrutura de árvore, onde as folhas são os objetos. </p>

_Figura 1.2: Exemplo do padrão Composite_
<br /><img src="docs/Assets/Img/Studies/EmergingDesignPatterns/CompositePatternExample.png" alt="Exemplo do padrão Composite"><br />
_Fonte: Gamma, Helm, Johnson, Vlissides, 1994, p. A-30_

_Código Fonte 1.2: Pseucodigo do padrão Composite em estado emergente_
```
class Figura {
    Figura[] atributo; // Deve ser um conjunto de elementos do tipo Figura
    void desenhar() {
        for (atributo.lenght()) {
            atributo.desenhar(); // Para cada elemento do conjunto
        }
    }
}
```
_Fonte: Job, 2014, p.34_

<p align="justify"> &emsp;&emsp; É possível perceber que a classe <code>Figura</code> tem o comportamento do padrão Composite, no entanto não segue a estruturação proposta pelo padrão.</p>

## State
<p align="justify"> &emsp;&emsp; O padrão <b>State</b> permite que um objeto mude seu comportamento conforme um estado interno. Por exemplo, uma classe <code>C</code> possui um atributo <code>a</code> que pode ser alterado a qualquer momento da execução dessa classe; Essa alteração é validada conforme o estado atual da classe e, após isso, atualizado, alterando o estado da classe.
<br /> &emsp;&emsp; No exemplo de <i>Código 1.3</i>, pode-se perceber que o comportamento do State é seguido, porém dentro de uma única função que trata todos estados possíveis. </p>

_Figura 1.3: Exemplo do padrão State_
<br /><img src="docs/Assets/Img/Studies/EmergingDesignPatterns/StatePatternExample.png" alt="Exemplo do padrão State"><br />
_Fonte: Gamma, Helm, Johnson, Vlissides, 1994, p. A-11_

_Código Fonte 1.3: Pseucodigo do padrão State em estado emergente_
```
class C{
    A state ;
    void m() {
        IF (state == "StateA" ){ //executa algo e muda o estado
            state ="StateB";
        }ELSE IF (state == "StateB" ){ //executa algo e muda o estado
            state ="StateC";
        }ELSE IF (state == "StateC "){ //executa algo e muda o estado
            state ="StateA";
        }
    )
} 
```
_Fonte: Job, 2014, p.33_

## Factory Method
<p align="justify"> &emsp;&emsp; O padrão <b>Factory Method</b> define uma interface para criação de objetos. A partir dela é possível instaciar objetos de outras subclasses definidas. </p>

_Figura 1.4: Exemplo do padrão Factory Method_
<br /><img src="docs/Assets/Img/Studies/EmergingDesignPatterns/FactoryMethodPatternExample.png" alt="Exemplo do padrão Factory Method"><br />
_Fonte: Gamma, Helm, Johnson, Vlissides, 1994, p. A-4_

<p align="justify"> &emsp;&emsp; O <i>Código Fonte 1.4</i> demonstra um padrão emergente derivado do Factory Method. Nele, a classe <code>StackTraceElementFactory</code> não possui uma subclasse definida para instanciar o objeto do tipo <code>StackTraceElement</code>, o que foge das restrições estruturais do padrão seguido.

_Código Fonte 1.4: O padrão Factory Method em estado emergente na classe ```StackTraceElementFactory```_
```
// Os imports , atributo s e demais métodos foram omitido s
public class StackTraceElementFactory {
    public StackTraceElement nativeMethodElement(String declaringClass, 
    String methodName) {
        return create(declaringClass, methodName, "Native", -2);
    }
    public StackTraceElement unknownSourceElement(String declaringClass, 
    String methodName) {
        return create(declaringClass, methodName, "Source", -1);
    }
    private StackTraceElement create(String declaringClass, String methodName, 
    String fileName, int lineNumber) {
        StackTraceElement result = new Throwable().getStackTrace()[0];
        setField(result, "declaringClass", declaringClass);
        setField(result, "methodName", methodName);
        setField(result, "fileName", fileName);
        setField(result, "lineNumber", new Integer(lineNumber));
        return result;
    }
} 
```
_Fonte: Job, 2014, p.29~30_

## Referências
* JOB, Ricardo de Sousa. Uma abordagem para detecção de padrões emergentes. Disponível em: <http://dspace.sti.ufcg.edu.br:8080/jspui/handle/riufcg/944>. Acessado em Outubro de 2020.
* LOVISCACH, Jörn. Design Patterns. Events. Disponível em: <https://doi.org/10.5446/9689>. Acessado em Outubro de 2020.
* GAMMA, Erich; HELM, Richard; JOHNSON, Ralph; VLISSIDES, John. Design Patterns: Elements of Reusable Object-Oriented Software Addison-Wesley Professional (1994).
* SERRANO, Milene. Arquitetura e Desenho de Software AULA - GRASP – PARTE I. Acessado em Outubro de 2020.