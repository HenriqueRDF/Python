# Análise de Dados do Super Bowl 🏈📊

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://python.org)
[![Pandas](https://img.shields.io/badge/Pandas-1.3.0-blue.svg)](https://pandas.pydata.org)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4.0-blue.svg)](https://matplotlib.org)
[![Seaborn](https://img.shields.io/badge/Seaborn-0.11.0-blue.svg)](https://seaborn.pydata.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org)
[![Licença](https://img.shields.io/badge/Licença-MIT-green.svg)](https://opensource.org/licenses/MIT)

Este projeto analisa dados históricos do Super Bowl para extrair insights sobre audiência televisiva, resultados dos jogos e shows do intervalo. O conjunto de dados inclui informações de 52 Super Bowls até 2018.

## 🔍 Conjuntos de Dados

1. **`super_bowls.csv`**: Detalhes dos jogos
   - Data, local, times participantes, placares
   - Pontos do vencedor e perdedor, diferença de pontos

2. **`tv.csv`**: Dados de audiência televisiva
   - Audiência média nos EUA
   - Custo dos comerciais

3. **`halftime_musicians.csv`**: Shows do intervalo
   - Artistas e bandas que se apresentaram
   - Número de músicas performadas

## 📊 Principais Resultados

### 1. Audiência Televisiva ao Longo do Tempo
```python
viewership_increased = False  # A audiência NÃO aumentou
```
- **Diminuição de 20%**: A audiência média caiu de 1.0 milhão (Super Bowl I) para 0.8 milhão (Super Bowl LII)
- Tendência de queda apesar do crescimento populacional dos EUA
- Possíveis fatores: fragmentação de audiência com streaming, mudança de hábitos de consumo

### 2. Jogos com Grande Diferença de Pontos
```python
difference = 1  # Apenas 1 jogo com diferença > 40 pontos
```
- **Super Bowl XXIV (1990)**: San Francisco 49ers 55 vs Denver Broncos 10
- Diferença de pontos: 45 pontos
- Curiosidade: Este foi o terceiro título do 49ers na década de 80

### 3. Artista Recordista nos Shows do Intervalo
```python
most_songs = "Justin Timberlake"  # Artista com mais músicas performadas
```
- **12 músicas** performadas em shows do intervalo
- Apresentações: Super Bowl XXXV (2001) e Super Bowl LII (2018)
- Outros destaques: Beyoncé (10 músicas), Diana Ross (10 músicas)

## 🛠️ Como Usar

### Pré-requisitos
- Python 3.8+
- Jupyter Notebook
---
**Nota**: Os gráficos e visualizações mencionados estão disponíveis no Jupyter Notebook do projeto.
