## Q1. Descreva o que é um Banco de Dados e o que é um Sistema Gerenciador de Banco de Dados. Cite exemplos de Bancos de Dados e seus SGBDs.
  ### Resposta:
  "Banco de Dados" é algo físico ou virtual que serve para guardar e gerenciar um conjunto de dados com contexto. Por exemplo:
  um diário é um banco de dados que contém dados relevantes e contextualizados sobre a vida de uma pessoa, já um banco de dados do "Mercado Livre" é um tipo de banco que contém dados
  relevantes para o sistema do "Mercado Livre".
  
  "Sistema Gerenciador de Banco de Dados" é um sistema que serve para interagir (criar, consultar, etc.) com o banco de dados mais facilmente e de forma segura e eficiente. Exemplos: MySQL
  Workbench, Oracle, MariaDB

## Q2. Quais os principais problemas de utilizar Sistemas de Arquivos para armazenagem de dados?
  ### Resposta:
  O primeiro deles é a possibilidade da existência de informações compostas por arquivos diferentes em formatos diferentes, assim, devido a falta de padronização, a consulta de
  informações é prejudicada. Além disso, outros dois problemas são a inconsistência e redundância de dados que podem ser causados pela falta de organização e comunificação entre os
  desenvolvedores, esse problema pode ser recorrente já que o modelo de "Sistemas de Arquivos" não oferece proteção inata contra isso. Outro problema é que determinadas operações devem
  acontecer em conjunto e como é difícil de garantir isso em um "Sistemas de Arquivos", o risco de uma dessas ações quebrar o banco não é baixo. Por fim, é complicado de separar o nível de
  acesso de cada pessoa que usa o banco em um sistema de arquivo, então alguém não autorizado pode ver informações confidenciais. 
