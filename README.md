# Sprint4-Modelagem-Linear-para-Aprendizado-de-Maquina

# Challenge Sprint IV — Modelagem Linear para Aprendizado de Máquina

## Descrição do projeto

Este projeto tem como objetivo aplicar técnicas de aprendizado de máquina para classificar dados relacionados à produção de energia renovável, utilizando um modelo de classificação linear desenvolvido em Python.

O trabalho utiliza o dataset Renewable Energy Production Dataset para realizar a análise exploratória dos dados, construir uma matriz de correlação, treinar um modelo de Regressão Logística e comparar seu desempenho em dois cenários de treinamento e teste.

## Objetivos

- Carregar e explorar o conjunto de dados em um DataFrame.
- Codificar a variável-alvo `Energy_Class`.
- Construir e analisar a matriz de correlação.
- Justificar a seleção das variáveis utilizadas no modelo.
- Implementar um classificador linear com Regressão Logística.
- Avaliar dois cenários de divisão dos dados: 60% para treinamento e 40% para teste; 85% para treinamento e 15% para teste.
- Analisar as matrizes de confusão e comparar acurácia, precisão e recall.
- Interpretar os resultados obtidos nos dois cenários.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Jupyter Notebook

## Estrutura do repositório

```text
Challenge-Sprint-IV/
│
├── Matrizes, métricas e gráficos/
│   ├── matriz_correlacao.png
│   ├── matriz_confusao_cenario1.png
│   ├── matriz_confusao_cenario2.png
│   ├── comparacao_cenarios.png
│   └── metricas_cenarios.csv
│
├── Challenge_Sprint_IV_Modelagem_Linear.ipynb
├── Renewable_Energy_Data.csv
└── README.md
```

A pasta `Matrizes, métricas e gráficos` reúne os resultados visuais e numéricos gerados durante a execução do notebook.

## Dataset

O projeto utiliza o arquivo `Renewable_Energy_Data.csv`, com dados relacionados à produção de energia renovável.

O conjunto de dados é utilizado para a preparação das informações, análise das relações entre as variáveis e treinamento do modelo de classificação.

## Metodologia

### 1. Preparação e análise dos dados

Inicialmente, o dataset é carregado em um DataFrame para permitir a exploração das informações. A variável-alvo `Energy_Class` é codificada para possibilitar sua utilização pelo algoritmo de aprendizado de máquina.

Em seguida, é construída uma matriz de correlação para investigar as relações lineares entre as variáveis numéricas e auxiliar na análise dos atributos.

### 2. Seleção das variáveis

A seleção dos atributos considera a análise da matriz de correlação e sua relação com a variável-alvo. As variáveis categóricas também são preparadas para utilização no modelo por meio da codificação apropriada.

### 3. Modelo de classificação linear

Foi utilizada a Regressão Logística, um algoritmo de classificação que combina as variáveis de entrada para estimar as classes de saída.

O modelo utiliza uma fronteira de decisão linear no espaço das características, permitindo separar as classes de acordo com os valores calculados a partir dos atributos.

### 4. Divisão dos dados

Foram avaliados dois cenários:

- **Cenário 1 — 60/40:** 60% dos dados são utilizados para treinamento e 40% para teste.
- **Cenário 2 — 85/15:** 85% dos dados são utilizados para treinamento e 15% para teste.

A comparação permite observar como a quantidade de dados utilizada no treinamento e no teste influencia os resultados do modelo.

### 5. Avaliação do modelo

O desempenho é avaliado por meio das seguintes métricas:

- **Acurácia:** proporção de previsões corretas em relação ao total de previsões.
- **Precisão:** avalia a proporção de previsões positivas corretas, considerando a média entre as classes.
- **Recall:** avalia a capacidade do modelo de identificar corretamente os exemplos de cada classe, considerando a média entre as classes.
- **Matriz de confusão:** permite visualizar as classificações corretas e os erros cometidos pelo modelo.

## Resultados

Os resultados da execução estão organizados na pasta `Matrizes, métricas e gráficos`.

- `matriz_correlacao.png`: apresenta as correlações entre as variáveis numéricas.
- `matriz_confusao_cenario1.png`: apresenta a matriz de confusão do cenário 60/40.
- `matriz_confusao_cenario2.png`: apresenta a matriz de confusão do cenário 85/15.
- `comparacao_cenarios.png`: apresenta a comparação visual das métricas dos dois cenários.
- `metricas_cenarios.csv`: contém os valores de acurácia, precisão, recall e tamanho do conjunto de teste.

Na execução realizada, o cenário 60/40 apresentou acurácia de 71,50%, precisão de 68,39% e recall de 63,67%, utilizando 400 registros no conjunto de teste.

O cenário 85/15 apresentou acurácia de 78,67%, precisão de 79,39% e recall de 74,82%, utilizando 150 registros no conjunto de teste.

Os resultados indicam que o cenário 85/15 apresentou métricas superiores nesta execução. Entretanto, seu conjunto de teste é menor, enquanto o cenário 60/40 permite avaliar o modelo com uma quantidade maior de registros.

## Como executar o projeto

1. Acesse o arquivo `Challenge_Sprint_IV_Modelagem_Linear.ipynb`.
2. Abra o notebook no Google Colab.
3. Disponibilize o arquivo `Renewable_Energy_Data.csv` no ambiente de execução, conforme o caminho utilizado no código.
4. Execute as células do notebook na ordem apresentada.
5. Observe a matriz de correlação, as matrizes de confusão e as métricas calculadas.
6. Compare os resultados dos cenários 60/40 e 85/15.

## Conclusão

O projeto possibilitou aplicar conceitos de aprendizado de máquina por meio da implementação de um classificador linear para dados relacionados à produção de energia renovável.

A comparação entre os cenários demonstrou diferenças nas métricas de avaliação. Nesta
