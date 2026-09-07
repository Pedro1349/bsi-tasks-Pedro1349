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
