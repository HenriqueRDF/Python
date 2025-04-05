# 🚴 Análise de Proximidade de Ciclovias - Baixada Santista

![Exemplo de Mapa Interativo](https://github.com/user-attachments/assets/7b29d044-f543-49a2-887a-26ef5862ebdc) *Mapa gerado pelo projeto*  
![Exemplo de Mapa Interativo 2](https://github.com/user-attachments/assets/98784b1d-d973-4dc2-a6a1-15f3e2572f97)  
*Santos, São Vicente*

Análise geoespacial para identificar pontos de interesse (POIs) distantes da rede cicloviária na região da Baixada Santista, SP.

## 🎯 Objetivo Ampliado

### Diagnóstico Espacial
Identificar **áreas críticas** com deficit de infraestrutura cicloviária através de análise geoespacial integrada:

```mermaid
graph TD
    A[Malha Cicloviária] --> B{Análise de Proximidade}
    C[Pontos de Interesse] --> B
    D[Vias Urbanas] --> B
    B --> E[Mapa de Calor de Deficits]
    E --> F[Priorização de Intervenções]
```
## 🌱 Histórico e Importância

### Origem Acadêmica
Este estudo nasceu como trabalho na **FATEC Baixada Santista**, desenvolvido inicialmente para a disciplina de:
- Projeto Integrador III

### Evolução do Projeto
```diff
# Versão Inicial (Trabalho em Grupo)
- Análise básica de proximidade
- Visualizações estáticas
- Dados limitados a 3 categorias de POIs

# Versão Atual (Desenvolvimento Individual)
+ Algoritmos otimizados
+ Mapas interativos com Folium
+ Expansão para 8 categorias de POIs
+ Metodologia reprodutível
```

## 🛠️ Tecnologias Utilizadas
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![GeoPandas](https://img.shields.io/badge/GeoPandas-0.10%2B-green)
![Folium](https://img.shields.io/badge/Folium-0.12%2B-orange)

```mermaid
graph TD
    A[Dados Geográficos] --> B{Processamento}
    B --> C[Análise de Distâncias]
    B --> D[Visualização]
    C --> E[POIs Distantes]
    D --> F[Mapa Interativo]
