# Detecção de Fraudes em Transações Financeiras com XGBoost

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.0.2-orange)](https://scikit-learn.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-1.5.1-green)](https://xgboost.readthedocs.io/)

Projeto de machine learning para identificar transações fraudulentas no dataset [Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) do Kaggle.

## 📊 Análise Visual

### 1. Matriz de Confusão
![Matriz de Confusão](https://github.com/user-attachments/assets/462d2f68-87d7-453d-9108-acea8e81c041)

- **Insight**: Alto número de verdadeiros negativos (84,145) e positivos (82,574), com poucos falsos positivos (1,004).

### 2. Curva Precision-Recall
![Curva Precision-Recall](https://github.com/user-attachments/assets/4438612c-99e2-4ca8-b22b-763aeed0814b)


- **AUC**: 0.98 (ideal para dados desbalanceados)
- **Insight**: Trade-off ótimo entre precisão e recall para fraudes.

### 3. Features Mais Importantes
![Feature Importance](https://github.com/user-attachments/assets/33dcda17-90f7-423b-9405-39b95863739c)


- **Top 3 features**:
  1. `V17` (PCA)
  2. `V14` (PCA) 
  3. `Amount` (valor da transação)

### 4. Distribuição de Valores por Classe
![Distribuição Amount](https://github.com/user-attachments/assets/90e241ab-a9d4-4b4d-bd37-06af7c2dfbc9)

- **Insight**: Transações fraudulentas tendem a ter valores menores.

## 📌 Resultados Principais
- **Precision (Fraudes):** 0.99  
- **Recall (Fraudes):** 0.97  
- **F1-Score:** 0.98  
- **AUC-PR**: 0.98

## 🛠️ Tecnologias
- **Linguagem**: Python 3.8+
- **Bibliotecas**:
  ```python
  pandas, scikit-learn, xgboost, imbalanced-learn, seaborn, matplotlib
