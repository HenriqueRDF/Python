
![Python Badge](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TensorFlow Badge](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras Badge](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![Status](https://img.shields.io/badge/Status-Concluído-green)

## 🎯 Visão Geral e Objetivo

Este projeto de **Deep Learning** visa classificar imagens do famoso dataset **CIFAR-10** em 10 categorias distintas. O foco técnico é a implementação de uma **Rede Neural Convolucional (CNN)**, servindo como uma demonstração prática avançada da **Álgebra Linear** no contexto de **Visão Computacional**.

O projeto detalha como as imagens são tratadas como **tensores** e como as operações convolucionais e de *pooling* funcionam como transformações e reduções de matrizes.

## 💾 Dataset

* **Nome:** CIFAR-10 (Canadian Institute for Advanced Research)
* **Fonte:** Keras / Kaggle
* **Conteúdo:** 60.000 imagens coloridas 32x32 em 10 classes (aviões, automóveis, pássaros, gatos, cervos, cachorros, sapos, cavalos, navios e caminhões).

## 🧠 Arquitetura e Matemática

A arquitetura implementada segue o padrão VGG simplificado, com blocos CONV-CONV-POOL.

| Camada | Função Matemática | Propósito |
| :--- | :--- | :--- |
| **Normalização** | Escalonamento de tensores [0-255] para [0-1] | Otimiza a convergência do Gradiente Descendente. |
| **Conv2D** | **Convolução** (Multiplicação de Matrizes/Tensores) | Aplica transformações lineares via filtros (kernels) para extrair features (bordas e texturas). |
| **MaxPooling2D** | **Subamostragem** (Redução de Dimensionalidade) | Reduz o tamanho dos mapas de features, tornando o modelo robusto a variações e translações. |
| **Dense (Saída)** | Multiplicação Matriz-Vetor e Softmax | Classifica o vetor de features final, gerando o vetor de probabilidade para as 10 classes. |

## 📈 Resultados do Treinamento

| Métrica | Valor |
| :--- | :--- |
| **Arquitetura** | CNN com Blocos Convolucionais (VGG Simplificada) |
| **Número de Épocas** | 50 |
| **Acurácia Final de Validação** | **78.73%** |
| **Loss Final de Validação** | 0.6896 |

<img width="1189" height="490" alt="Curvas" src="https://github.com/user-attachments/assets/9024a789-89a0-4e26-9381-d545542e2e8a" />


## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Deep Learning:** TensorFlow, Keras
* **Álgebra/Numérico:** NumPy
* **Visualização:** Matplotlib
