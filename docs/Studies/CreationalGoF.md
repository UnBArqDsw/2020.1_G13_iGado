# GoF's Criacionais

|    Data    | Versão |                Descrição                |                     Autor(es)                     |
| :--------: | :----: | :-------------------------------------: | :-------------------------------------------: |
| 10/10/2020 |  1.0   | Criação do estudo de GoFs Criacionais | [Guilherme Mendes](https://github.com/guilherme-mendes) |
| 10/10/2020 |  1.1   | Revisão do documento | [Lucas Fellipe](https://github.com/lucasfcm9) |
| 26/10/2020 |  1.2   | Refatoração do estudo de GoFs Criacionais | [Guilherme Mendes](https://github.com/guilherme-mendes) |
| 26/10/2020 | 1.3 | Revisão do documento | [João Pedro Guedes](https://github.com/sudjoao)|

<p align="justify"> &emsp;&emsp; Os GoF's são padrões de design que visam prover soluções para problemas recorrentes no desenvolvimento e manutenção de software orientado a objetos. Buscando sempre boas práticas de programação.</p>
<p align="justify"> &emsp;&emsp; Os Padrões de Design Criacionais (Creational Patterns) fornecem vários mecanismos de criação de objetos, que aumentam a flexibilidade e reutilização de código já existente.</p>

- Problemáticas:
  - Definir qual classe concreta deve ser utilizada para criar o objeto (instâncias de um objeto);
  - Definir como os objetos devem ser criados e como eles se relacionam com outros objetos do sistema.

- Principais GoF's Criacionais:
  - Factory Method
  - Abstract Method
  - Builder
  - Prototype
  - Singleton

### Factory Method

<p align="justify"> &emsp;&emsp; O Factory Method é um padrão criacional de projeto que fornece uma interface para criar objetos em uma superclasse e permitir delegar a instanciação às subclasses.</p>

<img src='docs/Assets/Img/Studies/GoFs/Creational/creational.png'>

- Vantagens:

  - Reutilização;
  - Manutenibilidade;
  - Coesão;
  - Dentre outros aspectos relevantes para a programação de sistemas OO.

- Exemplo de uso:

```python
import os
from flask import Flask
from flask_sqlalchemy import SQLAlchemy

# instantiate the db
db = SQLAlchemy()

def create_app(script_info=None):

    # instantiate the app
    app = Flask(__name__)

    # set config
    app_settings = os.getenv('APP_SETTINGS')
    app.config.from_object(app_settings)

    # set up extensions
    db.init_app(app)

    # register blueprints
    from project.api.example import example_blueprint
    app.register_blueprint(example_blueprint)

    # shell context for flask cli
    @app.shell_context_processor
    def ctx():
        return {'app': app, 'db': db}

    return app
```

### Abstract Factory

<p align="justify"> &emsp;&emsp; Permitir a criação de famílias de objetos relacionados ou dependentes por meio de uma única interface e sem que a classe concreta seja especificada.</p>

<img src='docs/Assets/Img/Studies/GoFs/Creational/creational1.png'>

- Vantagens:

  - Os produtos obtidos de uma fábrica são compatíveis entre si.
  - Evita um vínculo forte entre produtos concretos e o código cliente.
  - Extrair o código de criação do produto para um lugar, fazendo o código ser de fácil manutenção.
  - Introduzir novas variantes de produtos sem quebrar o código cliente existente.

- Exemplo de uso:

```jsx
interface GUIFactory is
    method createButton():Button
    method createCheckbox():Checkbox

class WinFactory implements GUIFactory is
    method createButton():Button is
        return new WinButton()
    method createCheckbox():Checkbox is
        return new WinCheckbox()
```

### Builder

<img src='docs/Assets/Img/Studies/GoFs/Creational/creational2.png'>

<p align="justify"> &emsp;&emsp; Separar o processo de construção de um objeto de sua apresentação e permitir a sua criação passo a passo. Diferentes tipos de objetos podem ser criados com implementações distintas de cada passo.</p>

- Vantagens:

  - Construção de objetos passo a passo, adiar as etapas de construção ou rodar etapas recursivamente.
  - Reutilização do código de construção quando construindo várias representações de produtos.
  - Isolamento do código de construção complexo da lógica de negócio do produto.

- Exemplo de uso:

  ```jsx
  class Builder(ABC):
  
      @abstractproperty
      def product(self) -> None:
          pass
  
      @abstractmethod
      def produce_part_a(self) -> None:
          pass
  
      @abstractmethod
      def produce_part_b(self) -> None:
          pass
  
      @abstractmethod
      def produce_part_c(self) -> None:
          pass
  
  class Director:
  
      def __init__(self) -> None:
          self._builder = None
  
      @property
      def builder(self) -> Builder:
          return self._builder
  
      @builder.setter
      def builder(self, builder: Builder) -> None:
          self._builder = builder
  
      def build_minimal_viable_product(self) -> None:
          self.builder.produce_part_a()
  
      def build_full_featured_product(self) -> None:
          self.builder.produce_part_a()
          self.builder.produce_part_b()
          self.builder.produce_part_c()
  
  if __name__ == "__main__":
  ```

### Prototype

<p align="justify"> &emsp;&emsp; Criação de novos objetos a partir da cópia de objetos existentes.</p>

<img src='docs/Assets/Img/Studies/GoFs/Creational/creational3.png'>

- Vantagens:

  - Clonar objetos sem acoplá-los a suas classes concretas.
  - Se livrar de códigos de inicialização repetidos em troca de clonar protótipos pré-construídos.
  - Produzir objetos complexos mais convenientemente.
  - Alternativa para herança quando lidar com configurações pré determinadas para objetos complexos.

- Exemplo de uso:

```jsx
abstract class Shape is
    field X: int
    field Y: int
    field color: string

    constructor Shape() is

    constructor Shape(source: Shape) is
        this()
        this.X = source.X
        this.Y = source.Y
        this.color = source.color
    
		abstract method clone():Shape
```

### Singleton

<p align="justify"> &emsp;&emsp; Criação de uma única instância de uma classe e fornecer um modo de recuperá-la.</p>

<img src='docs/Assets/Img/Studies/GoFs/Creational/creational6.png'>

- Vantagens:

  - Uma classe só terá uma única instância.
  - Um ponto de acesso global para aquela instância.
  - O objeto singleton é inicializado somente quando for pedido pela primeira vez.

- Exemplo de uso:

```python
from typing import Optional

class SingletonMeta(type):
	_instance: Optional[Singleton] = None
	
	def __call__(self) -> Singleton:
		if self._instance is None:
			self._instance = super().__call__()
		return self._instance 
class Singleton(meteclass->SingletonMeta):
	def some_business_logic(self):
		#code
```

### Multiton

<p align="justify"> &emsp;&emsp; Criação limitada de instancias para que haja um controle maior do que esta sendo consumido. </p>

<img src='docs/Assets/Img/Studies/GoFs/Creational/creational4.png'>


### Object Pool

<p align="justify"> &emsp;&emsp; Possibilita o reaproveitamentos de objetos. </p>

<img src='docs/Assets/Img/Studies/GoFs/Creational/creational5.png'>

### Referências

- LARMAN, Craig. Utilizando UML e Padrões: Uma Introdução a Análise e ao Projeto.
- Refactoring Guru. Design Patterns. [S. l.], 2020. Disponível em: [https://refactoring.guru/design-patterns](https://refactoring.guru/design-patterns). Acesso em: 09 out. 2020.
- SERRANO, Milene. Arquitetura e Desenho de Software AULA - GoFs Comportamentais. Acesso em: 10 out. 2020.