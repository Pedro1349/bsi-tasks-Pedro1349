## Q1. O modelo de dados entidade-relacionamento foi desenvolvido para facilitar o projeto de banco de dados, permitindo especificação de um esquema que representa a estrutura lógica geral de um banco de dados. Descreva os três elementos básicos de um Modelo Entidade Relacionamento (MER).
### Resposta:
  * **Entidade:** É um objeto que existe e é distinguível dos outros objetos. Além disso, esse objeto pode ser concreto ou abstrato.
  * **Atributo:** São as características que descrevem instâncias de uma entidade. Além disso, cada atributo possui um domínio, que é um conjunto de valores usados para representá-lo.
    - **Tipos de atributos:**
      - Simples: São atributos que não são uma informação composta (ex: idade, nome)
      - Composto: Contém sub-atributos que compõem o atributo (ex: o atributo endereço tem como sub-atributos: rua, bairro, cidade etc.)
      - Simplesmente valorados: Têm um único valor para uma instância de uma entidade (ex: idade)
      - Multivalorados: Possuem vários valores numa instância de uma entidade (ex: Telefone: residencial, comercial)
  * **Relacionamento:** São associações entre uma ou mais entidades.
    - **Tipos de relacionamentos:**
      - Auto-relacionamento: É um relacionamento com uma única entidade (ex: empregado supervisiona empregado)
      - Relacionamento binário: É um relacionamento entre duas entidades (ex: filme possui diretor)
      - Relacionamento não-binário: É um relacionamento entre mais de duas entidades (ex: fornecedor fornece produto para projeto)


## Q2. Pesquise sobre as várias notações possíveis para Diagramas ER e cite alguns exemplos de notações diferentes para o mesmo conceito (ex.: cardinalidade, entidade subordinada, etc.).
### Resposta:
  * **Notação de Chen**: Essa notação foi criada por Peter Chen em 1976. Ela foi a primeira notação criada e continua sendo uma das notações mais populares para modelos ER conceituais e lógicos. Por fim, as entidades são representadas por retângulos, os relacionamentos por losangos e os atributos por elipses.
  * **Notação UML**: É uma notação muito utilizada no desenvolvimento de sistemas e em ferramentas profissionais de modelagem. Ela não foi criada inicialmente para ser uma notação de
    diagramas ER, mas devido a sua popularidade, a notação UML também comoçou a ser usada em diagramas ER. As entidades são epresentadas como classes (retângulos com divisões internas), os
    atributos são listados dentro do retângulo com seus respectivos tipos de dados e os relacionamentos são representados por linhas retas.
  * **Notação Crow's Foot**: É uma das notações mais populares no ambiente profissional e nas ferramentas de software de modelagem. Ela foi criada no final da década de 1970 e tem um foco
    naleitura rápida da cardinalidade, tanto que seu nome deriva da aparência do símbolo que representa a cardinalidade "n" (que lembra o pé de um pássaro). As entidades são representadas
    por caixas, os atributos são listados dentro das caixas e os relacionamentos são representados por linhas.
  * **Exemplos de notações diferentes para o mesmo conceito**:
    - **Entidade**: Na notação de Chen é representada por um retângulo. Na Crow's Foot é representada por uma caixa. Na UML é representada por uma classe.
    - **Atributo:** Na notação de Chen, os atributos são representados por elipses. Na Crow's Foot, geralmente ficam dentro da caixa da entidade. Na UML, os atributos ficam dentro da
      classe.
    - **Cardinalidade 1:N**: Na notação de Chen é representada por "1:N". Na Crow's Foot é representada por "1" no lado 1 e pelo o símbolo de “pé de corvo” no lado N. Na UML é representada
      como "1..*".
