Análise de Sentimentos em E-commerce Brasileiro

Análise de sentimentos em avaliações de e-commerce brasileiro utilizando Python, Processamento de Linguagem Natural (NLP) e Machine Learning para classificar comentários de clientes e gerar insights de negócios.

## Objetivo do Projeto

O objetivo deste projeto é aplicar técnicas de NLP e um modelo preditivo para categorizar automaticamente o sentimento das avaliações de clientes (Positivo, Negativo ou Neutro) e otimizar a triagem na gestão de relacionamento com o consumidor.

## Conjunto de Dados

Brazilian E-Commerce Public Dataset by Olist (Olist Order Reviews Dataset).

## Ferramentas

- Python
- Pandas
- NLTK
- Scikit-Learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Principais Análises

- Limpeza e pré-processamento de dados textuais (remoção de stopwords, URLs e caracteres especiais).
- Transformação de vocabulário em matriz numérica (Vetorização TF-IDF).
- Treinamento e validação de modelo de classificação via Regressão Logística.
- Avaliação de desempenho através de matriz de confusão e relatório de métricas (Precision, Recall, F1-score).

## Principais Insights

- O modelo de classificação atingiu 84% de exatidão (accuracy) na categorização de dados inéditos.
- O algoritmo apresentou alta precisão na identificação dos extremos, isolando com eficiência as avaliações positivas (F1-score: 0.91) e negativas (F1-score: 0.81).
- Comentários neutros (nota 3) demonstraram alta ambiguidade natural, resultando em menor previsibilidade pela máquina.
- A recomendação estratégica de negócio é adotar um modelo de moderação híbrido: a Inteligência Artificial automatiza a triagem dos extremos (elogios e reclamações graves), enquanto as avaliações neutras são direcionadas para análise humana.

## Estrutura do Projeto

```text
analise-sentimentos-ecommerce/
├── analise_avaliacoes_olist.ipynb
├── README.md
└── .gitignore
