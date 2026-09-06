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

  ## Q3. Explique as propriedades ACID: atomicidade, consistência, isolamento e durabilidade. Para cada propriedade, descreva um exemplo prático no contexto de uma transferência bancária e explique o que aconteceria se o SGBD não garantisse essa propriedade.
  ### Resposta:
  A atomicidade garante que um conjunto de operações seja tratado como algo único, ou seja, todas as operações do conjunto devem ser totalmente concluídas ou todas seram canceladas.Exemplo:
  uma tranferência de dinheiro entre duas contas em um banco, caso não houvesse atomicidade e ocorresse um bug no sistema, o dinheiro poderia ser retirado de uma conta sem chegar à outra,
  já que cada operação seria independente.
  
  A consistência exige que toda modificação resulte em um banco de dados com o estado válido, ou seja, que os dados permaneçam corretos e de acordo com as regras do banco. Exemplo:
  caso um usuário queria retirar dinheiro da sua conta no banco, o saldo da conta deve diminuir pelo mesmo valor retirado, caso não houvesse consistência e ocorresse um bug no sistema,
  o saldo da conta poderia subir ou nem mesmo ser modificado.
  
  O isolamento impede que transações simultâneas se interfiram entre si e cada uma seja concluída de forma independente. Exemplo: caso um usuário do sistema queira ver o seu saldo ao mesmo   tempo que recebe 500R$, o sistema deve mostrar o saldo original da conta, pois não houvesse isolamento e os 500R$ não fossem creditados devido a um bug, o sistema mostraria um saldo
  incorreto ao usuário.
  
  Por fim, a durabilidade garante que um conjunto de operações confirmada permaneça registrada mesmo após falhas no sistema. Exemplo: uma transferência de R$ 500,00 é confirmada, a
  alteração dos saldos deve permanecer registrada mesmo que o banco fique sem energia logo em seguida, sem a durabilidade, esse dinheiro transferido seria perdido.

  ## Q4. Para cada cenário abaixo, indique qual(is) propriedade(s) ACID está(ão) em jogo e justifique sua resposta: a) Queda de energia no meio de uma transferência deixou o valor debitado da conta de origem, mas não creditado na conta de destino. b) Dois atendentes debitam, ao mesmo tempo, o mesmo saldo de uma conta. c) O sistema confirma a operação, mas após reiniciar o servidor o dado foi perdido. d) Uma transferência que levaria o saldo abaixo do limite permitido é rejeitada pelo banco.
  ### Resposta:
  A - Atomicidade não foi respeitada, pois apenas uma das operações do conjunto foi concluída e ambas não foram canceladas. Além disso, a consistência também foi violada ja que o saldo da
  conta de destino não foi creditado. Durabilidade foi respeitada, pois a operação que finalizou continou registrada. Por fim, não há indícios de que o isolamento não foi respeitado também.

  B - Não teve isolamento, pois duas operações simultâneas interferiram no mesmo saldo. Em relação a atomicidade, consistência e durabilidade, não há indícios de que foram desrespeitadas.

  C - A durabilidade foi desrespeitada, pois o dado foi perdido mesmo após a confirmação da operação. Em relação a atomicidade, consistência e isolamento, não há indícios de que foram
  desrespeitadas.

  D - A consistência foi respeitada, pois o banco rejeitou a transferência que deixaria o saldo abaixo do limite permitido, mantendo as regras do sistema. Em relação a atomicidade, 
  durabilidade e isolamento, não há indícios de que foram desrespeitadas.

