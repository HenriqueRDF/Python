# Projeto de Álgebra Linear Aplicada: Análise de Similaridade Semântica de Notícias

## Descrição do Projeto
Este projeto demonstra a aplicação de conceitos fundamentais da Álgebra Linear (Representação Vetorial, Produto Escalar e Ângulos) para quantificar a similaridade temática entre documentos textuais. Utilizamos a técnica TF-IDF (Term Frequency-Inverse Document Frequency) para transformar artigos de notícias em vetores em um espaço de alta dimensionalidade. A métrica de Similaridade de Cosseno (cos(θ)) é usada para medir o ângulo entre esses vetores, provando a correlação entre a proximidade geométrica e a semelhança de conteúdo.

## Requisitos de Entrega
O trabalho foi desenvolvido para atender aos requisitos de entrega da disciplina de Álgebra Linear e está formatado como um artigo científico para potencial submissão.

| Arquivo | Conteúdo | Requisito |
| :--- | :--- | :--- |
| **`trabalho_alg_lin.py`** | Código Python completo, incluindo TF-IDF, cálculo de cosseno, PCA e amostragem estratificada. | **Obrigatório (.py)** |
| **`trabalho_alg_lin.tex`** | Código-fonte LaTeX (Times New Roman 12, Espaçamento 1.5, NBR 6022/APA) do artigo. | **Obrigatório (.tex)** |
| **`analise_vetorial.pdf`** | Artigo científico compilado (a ser gerado a partir do `.tex`). | **Obrigatório (.pdf)** |
| **`pca_cluster_tfidf_estratificado.png`** | Figura gerada pelo código Python, essencial para a prova geométrica do artigo. | **Suporte** |

## Dataset
* **Fonte:** Notícias publicadas no Brasil (Kaggle)
* **Link:** `https://www.kaggle.com/datasets/diogocaliman/notcias-publicadas-no-brasil`
* **Amostragem:** Foi utilizada Amostragem Aleatória Estratificada (14 documentos de 'economia', 'esportes', 'política') para mitigar o vício de dados e garantir a validade estatística e visualização do PCA.

## Tecnologias Utilizadas
* **Linguagem:** Python
* **Pacotes:** `pandas`, `sklearn` (`TfidfVectorizer`, `cosine_similarity`, `PCA`), `numpy`, `matplotlib`.

## Resultados Chave no Artigo
* **Colinearidade (Máxima Similaridade):** Ângulo de $16.09^\circ$ (cos($\theta$) = 0.9608), provando que o vocabulário é quase idêntico.
* **Ortogonalidade (Mínima Colinearidade):** Ângulo de $74.53^\circ$ (cos($\theta$) = 0.2667), provando a divergência temática no espaço vetorial.