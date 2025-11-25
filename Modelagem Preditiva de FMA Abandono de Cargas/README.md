# 🚢 FMA Analytics: Previsão de Abandono de Cargas com Survival Analysis

![Status](https://img.shields.io/badge/Status-Concluído-success)
![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Lib](https://img.shields.io/badge/Library-Lifelines-orange)
![Domain](https://img.shields.io/badge/Domain-Logística%20Portuária-green)

> **Uma abordagem de Data Science para prever riscos de perdimento (FMA) em recintos alfandegados, utilizando Simulação de Monte Carlo e Modelagem de Cox.**

---

## 📋 Sobre o Projeto

O abandono de cargas (FMA - Falta de Manifestação Aduaneira) é um dos maiores gargalos logísticos e jurídicos em zonas portuárias. Os relatórios tradicionais oferecem apenas uma visão retroativa ("quantas cargas foram abandonadas").

Este projeto propõe uma mudança de paradigma: **sair da análise descritiva para a preditiva**.

Utilizando dados reais de movimentação do Porto de Santos (ABTRA) e técnicas de **Bioestatística aplicadas à Logística**, desenvolvemos um motor capaz de simular cenários econômicos e legislativos para antecipar colapsos operacionais.

---

## 🎯 O Problema de Negócio

1.  **Dados Agregados:** As fontes públicas fornecem apenas totais mensais, impedindo a aplicação direta de Machine Learning.
2.  **Cegueira Operacional:** Gestores sabem o passado, mas não conseguem quantificar o risco das cargas atualmente no pátio.
3.  **Incerteza Legislativa:** Não existiam ferramentas para medir o impacto financeiro de alterações nos prazos legais (ex: redução de 90 para 60 dias).

---

## ⚙️ A Solução (Pipeline Técnico)

O projeto foi estruturado em 5 etapas rigorosas:

### 1. Engenharia de Dados (ETL & Silver Layer)
* **Desafio:** Dados brutos em Excel não estruturado (cabeçalhos visuais, rodapés).
* **Solução:** Pipeline de limpeza automatizado que gera arquivos CSV auditáveis e padronizados, garantindo integridade e reprodutibilidade.

### 2. Data Factory (Simulação de Monte Carlo)
* **Desafio:** Necessidade de dados granulares (linha a linha) para análise de sobrevivência.
* **Solução:** Aplicação de algoritmos estocásticos para transformar 164 registros mensais em um dataset com **+4 milhões de movimentações simuladas**.
* **Técnica:** Utilização de distribuição **Log-Normal** para simular tempos de permanência realistas (cauda longa).

### 3. Validação (Kaplan-Meier)
* Estimativa da curva de sobrevivência $S(t)$ da carga desovada.
* **Resultado:** O modelo validou o **"Abismo dos 90 Dias"**, demonstrando aderência total ao **Decreto nº 6.759/2009** (Regulamento Aduaneiro).

### 4. Inteligência Preditiva (Cox Proportional Hazards)
* Modelagem multivariada para medir o impacto da variável **Dólar (Câmbio)** no risco.
* **Insight:** Identificado *Hazard Ratio* de `0.86`, indicando que em períodos de crise cambial (Dólar alto), a eficiência logística tende a aumentar (proteção de caixa do importador).

### 5. Prescrição de Cenários (What-If Analysis)
* Simulação de impacto da redução do prazo legal de 90 para 60 dias.
* **Entrega:** Visualização da **"Zona de Risco Extra"**, quantificando o volume de carga que seria impactado pela mudança na lei.

---

## 📊 Resultados Visuais

*(Espaço reservado para as imagens geradas no Notebook)*

| Curva de Sobrevivência (Atual) | Simulação de Cenários (90 vs 60 Dias) |
|:---:|:---:|
| ![Kaplan Meier](https://via.placeholder.com/400x250?text=Inserir+Grafico+Kaplan) | ![Cenarios](https://via.placeholder.com/400x250?text=Inserir+Grafico+Cenarios) |

> *A área amarela no gráfico de cenários representa o volume financeiro e operacional em risco caso a legislação seja alterada.*

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Manipulação de Dados:** Pandas, NumPy
* **Estatística & Survival Analysis:** `lifelines` (Kaplan-Meier, CoxPHFitter)
* **Visualização:** Matplotlib

---

## 🚀 Como Executar

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/fma-analytics.git](https://github.com/seu-usuario/fma-analytics.git)
    ```
2.  **Instale as dependências:**
    ```bash
    pip install pandas numpy matplotlib lifelines openpyxl
    ```
3.  **Execute o Notebook:**
    Abra o arquivo `FMA_Survival_Analysis.ipynb` no Jupyter ou Google Colab.
    * *Nota:* O notebook inclui uma etapa de geração de dados sintéticos; portanto, não é necessário o arquivo original da ABTRA para rodar a demonstração, embora o código de ingestão esteja preservado.

---

## 👨‍💻 Autor

**[Seu Nome]**
* [LinkedIn](https://linkedin.com/in/seu-perfil)
* [Portfólio](https://seu-site.com)

---

> *"Transformando dados estáticos em gestão de risco dinâmica."*