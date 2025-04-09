# 🏡 Previsão de Preço de Casas - Seattle House Sales

Este projeto aplica técnicas de Machine Learning para prever o preço de venda de casas em Seattle, utilizando um conjunto de dados obtido via Kaggle. A análise inclui desde o carregamento dos dados até a construção de um modelo de regressão linear.

## 📂 Dataset

- Fonte: [Kaggle - House Sales in King County, USA](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)
- A base contém informações como:
  - Número de quartos e banheiros
  - Área construída e do terreno
  - Ano de construção
  - Localização (zipcode)
  - Condição geral do imóvel, entre outros

## 🛠️ Tecnologias e Bibliotecas

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (Regressão Linear, Métricas de Avaliação)

## ⚙️ Etapas Realizadas

1. **Importação e Leitura dos Dados**
2. **Análise Exploratória de Dados (EDA)**
3. **Limpeza de Dados**
4. **Seleção de Features**
5. **Divisão entre treino e teste**
6. **Treinamento do Modelo de Regressão Linear**
7. **Avaliação com métricas (R², RMSE, MAE)**

## 🧠 Modelo Utilizado

- **Regressão Linear** com `scikit-learn`

## 📊 Métricas de Avaliação

As métricas utilizadas para avaliar a performance do modelo foram:
- Coeficiente de Determinação (R²)
- Erro Médio Absoluto (MAE)
- Raiz do Erro Quadrático Médio (RMSE)
