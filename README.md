# Modelo de Previsão Limite de Cartão de Crédito para a FinTech Nova Geração utilizando XGBoost no AWS

## Problema de Negócio
A FinTech Nova Geração enfrenta desafios significativos na determinação do limite de crédito de cartão para novos clientes, resultando em atribuições inadequadas que podem levar tanto à concessão excessiva quanto à insuficiência de crédito. Para melhorar a precisão e eficiência dessa análise, a instituição busca desenvolver um modelo de machine learning que automatize o processo de determinação do limite de crédito de cartão para cada cliente.

## Detalhes do Problema
Atualmente, o processo manual de definição do limite de crédito de cartão da FinTech Nova Geração é propenso a erros humanos e inconsistências, resultando em limites de crédito inadequados. Limites de crédito mal atribuídos podem levar a riscos financeiros elevados ou à insatisfação dos clientes. A automação deste processo através de um modelo de machine learning pode não apenas acelerar a análise, mas também aumentar a precisão na determinação dos limites de crédito de cartão, reduzindo os riscos associados.

## Insights da Codificação
A seguir está o processo completo de codificação usado para desenvolver o modelo de machine learning utilizando o algoritmo XGBoost no AWS ( Amazom Web Services)

## Importação de Bibliotecas
Primeiro, é feito as importações das bibliotecas necessárias:

------------------------------

## Carregamento e processamento dos Dados

------------------------------

## Análise descritiva e visualização

-------------------------

## Divisão da base de dados em treinamento e teste

--------------------------

## Salvando as bases de treinamento e teste

-------------------------

## Configurações SageMaker

---------------------

## Treinamento do XGBoost

-----------------------

## Deploy, previsões e avaliação
-------------------------------


## Principais Pontos Abordados:
1 - Importação dos Dados:
Leitura do arquivo

2 - Limpeza e Pré-processamento:
Remoção de colunas desnecessárias.
Criação de novas colunas (BILL_TOTAL e PAY_TOTAL) a partir de somas de outras colunas.
Remoção de colunas intermediárias após a criação das novas colunas.

 3 - Divisão dos Dados:
Separação dos dados em conjuntos de treinamento (21000 linhas) e teste (9000 linhas).

4- Visualização de Correlação:
Geração de um mapa de calor para visualizar a correlação entre variáveis.

5 - Treinamento e Teste:
Criação e separação das variáveis independentes (X_teste) e dependentes (y_teste).
Salvamento dos Dados:
Salvamento das bases de treinamento e teste.

6 - Deploy e Previsão com Modelo:
Implementação de um modelo XGBoost.
Previsão nos dados de teste e avaliação do modelo.

7 - Avaliação do Modelo:
Cálculo das métricas de erro: MAE, MSE e RMSE.

8 - Encerramento:
Exclusão do endpoint do modelo no AWS.


## Conclusão e Resumo dos Resultados:

O modelo XGBoost treinado apresentou um desempenho razoável, com um MAE (Erro Médio Absoluto) de 76.552,94, um MSE (Erro Quadrático Médio) de 10.886.941.880,65 e um RMSE (Raiz do Erro Quadrático Médio) de 104.340,51. Embora o erro seja relativamente alto, o modelo conseguiu prever valores com um grau de precisão aceitável dado a complexidade dos dados de crédito.
A análise de correlação entre variáveis e a subsequente redução de dimensionalidade permitiram a criação de um modelo mais simplificado e eficiente. A divisão dos dados em conjuntos de treinamento e teste garantiu uma validação adequada da performance do modelo.
Com ajustes adicionais nos hiperparâmetros e possíveis otimizações, espera-se que a acurácia do modelo possa ser ainda mais aprimorada, contribuindo significativamente para a tomada de decisões na análise de crédito.
