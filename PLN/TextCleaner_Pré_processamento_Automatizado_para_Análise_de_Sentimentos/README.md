# 🧹 TextCleaner - Pré-processamento Automatizado para Análise de Sentimentos

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![NLTK](https://img.shields.io/badge/NLTK-3.6.5-green)
![GitHub Last Commit](https://img.shields.io/github/last-commit/seuuser/TextCleaner)

Ferramenta de pré-processamento de textos em português para projetos de NLP, com remoção de stopwords, normalização e tokenização inteligente.

## ✨ Features
- ✅ Limpeza de pontuação e emojis
- ✅ Tokenização específica para português
- ✅ Filtragem de stopwords personalizável
- ✅ Processamento em lote para grandes volumes

## 🚀 Como Usar
```python
from textcleaner import preprocess

textos = ["Ótimo produto! Adorei 😊", "Péssimo atendimento!"]
clean_texts = [preprocess(t) for t in textos]
# Resultado: [['ótimo', 'produto', 'adorei'], ['péssimo', 'atendimento']]
