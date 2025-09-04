# Projeto de EDA – California Housing e Chipotle


## 1. Visão Geral
Este projeto realiza uma análise exploratória de dados (EDA) em dois conjuntos de dados distintos:


1. **California Housing** – Dados de imóveis da Califórnia, extraídos via `sklearn.datasets.fetch_california_housing`.
2. **Chipotle Orders** – Dados de pedidos da rede Chipotle, contendo informações de produtos, preços e quantidade.


O objetivo é entender a distribuição dos dados, identificar padrões, detectar outliers e gerar insights iniciais para análises ou modelos futuros.

## 2. Datasets


### 2.1 California Housing
- **Origem:** [sklearn.datasets.fetch_california_housing](https://scikit-learn.org/stable/datasets/real_world.html#california-housing-dataset)
- **Colunas principais:**
- `MedInc` – Renda mediana do bloco.
- `HouseAge` – Idade média das casas no bloco.
- `AveRooms` – Número médio de cômodos por residência.
- `AveBedrms` – Número médio de quartos por residência.
- `Population` – População do bloco.
- `AveOccup` – Ocupação média por residência.
- `Latitude` / `Longitude` – Coordenadas geográficas.
- `MedHouseVal` – Valor mediano da casa (target).


### 2.2 Chipotle 
- **Origem:** [Dataset público do Chipotle]([https://raw.githubusercontent.com/justmarkham/DAT8/master/data/chipotle.tsv])
- **Colunas principais:**
- `order_id` – Identificador do pedido.
- `quantity` – Quantidade de cada item no pedido.
- `item_name` – Nome do produto.
- `choice_description` – Descrição das escolhas adicionais.
- `item_price` – Preço do item.


## 3. Análises Realizadas
Para ambos os datasets, foram conduzidas as seguintes análises:


### 3.1 Limpeza e pré-processamento
- Tratamento de valores ausentes e duplicados.
- Conversão de tipos de dados (ex.: preço para float).


### 3.2 Estatísticas descritivas
- Média, mediana, desvio padrão e quartis.
- Distribuição de variáveis numéricas e categóricas.


### 3.3 Visualizações
- Histogramas e boxplots para entender a distribuição e detectar outliers.
- Heatmaps de correlação (California Housing).
- Gráficos de barras para frequência de produtos (Chipotle).


### 3.4 Insights preliminares
- Relação entre idade das casas, renda e valor médio das casas (California Housing).
- Produtos mais vendidos e análise de preços (Chipotle).
