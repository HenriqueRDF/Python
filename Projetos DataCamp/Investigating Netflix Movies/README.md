# 🎬 Investigando Filmes da Netflix dos Anos 90

[![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458?logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-DataViz-3C5488?logo=plotly&logoColor=white)](https://seaborn.pydata.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Graphs-orange?logo=matplotlib&logoColor=white)](https://matplotlib.org/)
[![Status](https://img.shields.io/badge/Status-Completed-brightgreen)]()
[![License](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)

> Projeto de análise exploratória de dados (EDA) realizado na plataforma [DataCamp](https://www.datacamp.com/) com foco em padrões de duração e gênero nos filmes da Netflix lançados na década de 1990.

---

## 📌 Descrição

Neste projeto, investigamos dados sobre os filmes adicionados à Netflix e lançados entre 1990 e 1999. A proposta é explorar estatísticas de duração e entender comportamentos de gêneros populares como ação.

---

## 🧰 Tecnologias utilizadas

- **Python 3.10**
- **Pandas**
- **Seaborn**
- **Matplotlib**
- **Jupyter Notebook**

---

## ⚙️ Etapas do projeto

- 📥 Importação e pré-processamento do dataset `netflix_data.csv`
- 🧹 Limpeza e conversão de colunas
- 🎯 Filtragem dos filmes da década de 1990
- 📊 Visualização da distribuição de duração dos filmes
- 🔎 Análise de filmes de ação com menos de 90 minutos
- 💡 Extração de insights estatísticos

---

## 📈 Resultados

🎬 **Duração mais frequente:** `94 minutos`  
Filmes lançados nos anos 90 tendem a ter cerca de 1h34min, mantendo um equilíbrio entre ritmo e desenvolvimento narrativo.

🔥 **Filmes de ação com menos de 90 minutos:** `7 filmes`  
Produções curtas de ação são minoria, o que sugere que o gênero costuma exigir mais tempo de tela para cenas complexas.

✅ **Conclusão geral:**  
Há uma clara preferência por filmes de **duração intermediária** na década de 1990, e uma escassez de títulos de ação curtos nesse período.

---

## 📁 Como visualizar

Você pode abrir o notebook no [Google Colab](https://colab.research.google.com/) ou executar localmente com:

```bash
git clone https://github.com/seu-usuario/projeto-netflix-datacamp.git
cd projeto-netflix-datacamp
jupyter notebook
