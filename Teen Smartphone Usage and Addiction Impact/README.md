# 📱 Análise do Uso de Smartphone por Adolescentes e Impactos Potenciais
> Teen Smartphone Usage & Potential Impact Analysis

[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-blue?logo=pandas)](https://pandas.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?logo=matplotlib)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Stats%20Plots-lightblue?logo=python)](https://seaborn.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Clustering-brightgreen?logo=scikit-learn)](https://scikit-learn.org/)
[![Kaggle Dataset](https://img.shields.io/badge/Dataset-Kaggle-blue?logo=kaggle)](https://www.kaggle.com/datasets/sumedh1507/teen-phone-addiction)

## 📊 Sobre o Projeto

Este projeto explora padrões de uso de smartphones por adolescentes, visando identificar possíveis perfis de usuários e impactos comportamentais relacionados ao vício digital. A análise foi realizada utilizando técnicas de pré-processamento, redução de dimensionalidade e clustering não supervisionado.

O dataset foi obtido no [Kaggle](https://www.kaggle.com/datasets/sumedh1507/teen-phone-addiction), contendo dados anonimizados de adolescentes sobre hábitos digitais, uso de aplicativos, dependência, sono e saúde.

---

## 🧠 Objetivo

Investigar como diferentes perfis de adolescentes utilizam o smartphone e como isso pode estar associado a riscos como dependência digital, queda no desempenho escolar ou impactos em saúde mental e física.

---

## 🔍 Metodologia

- **Limpeza e pré-processamento dos dados**
- **Seleção de variáveis relacionadas ao uso do smartphone**
- **Escalonamento dos dados com StandardScaler**
- **Redução de dimensionalidade com PCA**
- **Clusterização com K-Means**
- **Validação dos clusters com Silhouette Score e método do cotovelo**
- **Criação de perfis comportamentais baseados nos clusters**

---

## 📌 Resultados e Descobertas

Identificamos **4 clusters** com perfis distintos de uso:

| Cluster | Nome do Perfil                       | Características principais |
|--------:|--------------------------------------|----------------------------|
| 0       | **Notificadores compulsivos**        | Verificam o celular com altíssima frequência diária, possível relação com ansiedade |
| 1       | **Usuários equilibrados e produtivos**| Uso moderado, maior tempo em apps educacionais, menor tempo em jogos |
| 2       | **Gamers intensos / App-centric**     | Alto tempo em apps e jogos, pouco foco educacional |
| 3       | **Usuários casuais / Baixo uso**      | Baixa interação geral, menor risco de dependência |

Além disso, foram observados:

- A aplicação de **PCA** indicou clara separação entre clusters.
- O **Silhouette Score** médio foi satisfatório (~0.47), validando a segmentação.

---

## 🔎 Próximos Passos

- Explorar relações entre clusters e variáveis de saúde mental, desempenho acadêmico e qualidade do sono.
- Avaliar intervenções direcionadas com base nos perfis.

---

## 🚀 Tecnologias e Bibliotecas

- Python 3.10
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-Learn
- Jupyter Notebook

---

## 📂 Como usar

Clone este repositório e execute o notebook:

```bash
git clone https://github.com/seu-usuario/Teen-Smartphone-Usage.git
cd Teen-Smartphone-Usage
jupyter notebook
