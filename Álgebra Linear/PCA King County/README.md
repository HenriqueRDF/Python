# 🏡 Otimização de Regressão com PCA: Redução de Dimensionalidade no Mercado Imobiliário de King County 📊

![Python Badge](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Scikit-learn Badge](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![NumPy Badge](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-green)

## 🎯 Objetivo do Projeto

Este projeto demonstra a aplicação prática da **Análise de Componentes Principais (PCA)** para otimizar um modelo de Regressão Linear. O foco foi encontrar o *trade-off* ideal entre a complexidade do modelo (número de *features*) e sua performance preditiva no mercado de imóveis de King County (Seattle).

A principal contribuição é a análise de **Álgebra Linear** (Autovalores e Autovetores) para reduzir o espaço vetorial de dados sem comprometer significativamente a precisão.

## 💾 Dataset

O conjunto de dados utilizado é amplamente conhecido na área de Machine Learning para Regressão.

* **Nome:** House Sales in King County, USA
* **Fonte:** [Kaggle](https://www.kaggle.com/datasets/harlfoxem/housesalesprediction)
* **Descrição:** Contém dados de vendas de casas na área de King County, Washington, incluindo Seattle, entre maio de 2014 e maio de 2015. A variável alvo (`target`) é o preço (`price`).
* **Uso:** O dataset é acessado diretamente no notebook via `kagglehub` para garantir a reprodutibilidade.

## ⚙️ Metodologia Técnica e Matemática

A solução foi dividida nas seguintes etapas, com destaque para a aplicação da matemática subjacente:

1.  **Pré-processamento:** Limpeza de dados categóricos (One-Hot Encoding em `zipcode`) e **Escalonamento** (`StandardScaler`) das features. *O escalonamento é obrigatório antes do PCA.*
2.  **Modelo Baseline:** Treinamento de uma Regressão Linear no dataset original (87 features) para estabelecer a métrica de comparação.
3.  **Análise PCA (O Coração da Álgebra Linear):**
    * Cálculo dos **Autovalores e Autovetores** da Matriz de Covariância.
    * Análise da **Variança Acumulada Explicada** via *Scree Plot*.
4.  **Redução de Dimensionalidade:** Seleção do número ótimo de componentes para reter **95% da variância**.
5.  **Modelo Otimizado:** Treinamento do mesmo modelo de Regressão Linear no dataset transformado pelo PCA.

## 📊 Resultados e Análise do Trade-off

A análise da variância acumulada (Scree Plot) indicou que a maior parte da informação dos dados estava concentrada em um subespaço de menor dimensão.

| Métrica | Baseline (87 Features) | Otimizado (73 Componentes) |
| :--- | :--- | :--- |
| **Dimensionalidade Reduzida** | N/A | **16.09%** |
| **R² Score** | **0.8081** | **0.7814** |
| **RMSE (Erro Médio)** | R\$ 170.329,55 | R\$ 181.809,50 |

### **Conclusão:**

O PCA permitiu uma redução de dimensionalidade de **16.09%** (de 87 para 73 features), o que se traduz em um modelo mais rápido e eficiente em termos de custo computacional. A perda de $2.67\%$ no $R^2$ (de 0.8081 para 0.7814) é um *trade-off* aceitável e muitas vezes preferível em cenários de produção de larga escala, onde a velocidade de inferência é crítica.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.x
* **Manipulação de Dados:** `pandas`, `numpy`
* **Machine Learning/Estatística:** `scikit-learn` (`LinearRegression`, `StandardScaler`, `PCA`)
* **Visualização:** `matplotlib`, `seaborn`
