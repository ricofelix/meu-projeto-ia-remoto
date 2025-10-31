Trabalho ML



Turma ADA 1486



LEANDRO FELIX RODRIGUES

LEANNDROF@GMAIL.COM



Projeto de Previsão de Empréstimo Pessoal

Descrição do Problema

O projeto tem como objetivo desenvolver um modelo capaz de prever quais clientes de um banco têm maior probabilidade de aceitar uma oferta de empréstimo pessoal. Esse tipo de solução é bastante útil para direcionar campanhas e ofertas, aumentar a taxa de adesão e evitar desperdício de recursos com clientes pouco propensos a contratar esse serviço.



Detalhes da Base de Dados

Foi utilizada uma base de dados pública de clientes bancários, contendo cerca de 5.000 registros. Cada linha representa um cliente e traz informações como idade, renda anual, tempo de experiência profissional, tamanho da família, média de gastos mensais no cartão de crédito, nivel de escolaridade, valor de hipoteca e a presença de diferentes tipos de contas e serviços bancários.

A coluna de interesse é “Personal Loan”, que indica se o cliente contratou (1) ou não contratou (0) o empréstimo.



Principais variáveis da base:

Age: idade do cliente



Experience: tempo de experiência profissional (anos)



Income: renda anual



Family: tamanho da família



CCAvg: gasto médio mensal no cartão de crédito



Education: nível educacional



Mortgage: valor de hipoteca



Personal Loan: contratou empréstimo (alvo do modelo)



Demais colunas binárias: presença de serviço online, cartão de crédito, conta de depósito etc.



Metodologia do Experimento

O trabalho começou com o tratamento inicial dos dados – limpeza para remover duplicidades, normalização das variáveis contínuas e separação do conjunto em treino e teste.

Foram testados dois algoritmos de classificação bem conhecidos (Árvore de Decisão e Random Forest), escolhidos por serem facilmente interpretáveis e eficazes para esse perfil de dados.



O desempenho dos modelos foi avaliado principalmente pela métrica AUC-ROC, mais adequada para problemas de classificação desequilibrada como esse, além da acurácia.

Os hiperparâmetros dos modelos foram otimizados usando a técnica de validação cruzada, garantindo confiabilidade no resultado sem “vicio” ao conjunto de treino.



Após a comparação, foi escolhida a abordagem que apresentou os melhores resultados, pronta para ser testada em produção e eventualmente integrada ao sistema do banco.

