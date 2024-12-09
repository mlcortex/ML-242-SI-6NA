# Equipe "EQUIPE_CPU"

## Equipe (max 4 pessoas):
- Guilherme Kauã Diniz Cabral - 01549420.
- Eduarda Martins do Nascimento - 01525081.
- Bruno Belarmino da Silva - 24010424.
- Jonas Ferreira da Silva - 01063866.
- José Darlan de Lima Carvalho - 01466857.

# Nome projeto
Tecnica Árvore de Decisão para Regressão

# Tema
Este programa usa aprendizado de máquina para prever o preço de CPUs.

## Base de dados
https://www.kaggle.com/datasets/iliassekkaf/computerparts

## Modelo/Alg.
Árvore de Decisão para Regressão

## Objetivos
prever o preço de CPUs.

## Etapas de modelagem
As etapas da modelagem, são:

1. Coleta de Dados:
    - Download do dataset do Kaggle.
    - Especificação do arquivo CSV a ser utilizado.

2. Carregamento dos Dados:
    - Leitura do arquivo CSV em um DataFrame pandas.
    - Visualização das primeiras linhas do DataFrame para inspeção inicial.

3. Pré-processamento dos Dados:
    - Conversão de valores de string para numérico (frequência do processador).
    - Remoção de linhas com valores ausentes na coluna 'Processor_Base_Frequency'.

4. Divisão dos Dados em Treinamento e Teste:
    - Separação dos dados em conjuntos de treinamento e teste usando train_test_split.
    - Definição de recursos (features, X) e variável alvo (target, y).

5. Pré-processamento Adicional:
    - Aplicação de OneHotEncoder para variáveis categóricas.
    - Aplicação de StandardScaler para variáveis numéricas.
    - Utilização de ColumnTransformer para aplicar transformações consistentemente.

6. Treinamento do Modelo:
    - Inicialização de um modelo DecisionTreeRegressor.
    - Treinamento do modelo com os dados de treinamento pré-processados.

7. Avaliação do Modelo:
    - Previsões com o modelo treinado usando os dados de teste.
    - Cálculo de métricas de desempenho: Mean Squared Error (MSE) e R² Score.

8. Resultados do Modelo Resumidos:
    - Interpretação das métricas de desempenho (MSE e R²).