# Análise de Sentimentos em E-commerce Brasileiro

Análise de sentimentos em avaliações de e-commerce brasileiro utilizando Python, Processamento de Linguagem Natural (NLP) e Machine Learning para classificar comentários de clientes e gerar insights de negócios.

## Objetivo do Projeto

Aplicar técnicas de NLP e um modelo preditivo para categorizar automaticamente o sentimento das avaliações de clientes (Positivo, Negativo ou Neutro) e otimizar a triagem na gestão de relacionamento com o consumidor.

## Conjunto de Dados

Brazilian E-Commerce Public Dataset by Olist (Olist Order Reviews Dataset), com 99.224 avaliações, das quais 40.977 têm comentário em texto e foram usadas no projeto.

O sentimento foi definido a partir da nota da avaliação: notas 1 e 2 = Negativo, nota 3 = Neutro e notas 4 e 5 = Positivo. A base é desbalanceada: 65% positivas, 27% negativas e 9% neutras.

Os dados estão disponíveis no Kaggle (busque por "Brazilian E-Commerce Public Dataset by Olist"). Baixe o arquivo `olist_order_reviews_dataset.csv` e coloque-o na pasta `data/raw/` para rodar o notebook.

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
- Transformação de vocabulário em matriz numérica (vetorização TF-IDF com 5.000 atributos).
- Treinamento e validação de modelo de classificação via Regressão Logística (80% treino e 20% teste).
- Avaliação de desempenho através de matriz de confusão e relatório de métricas (Precision, Recall, F1-score).

## Principais Insights

- O modelo atingiu 84% de exatidão (accuracy) nos dados de teste. Uma previsão que sempre escolhesse "Positivo" acertaria cerca de 65%.
- Alta capacidade de identificar os extremos: avaliações positivas (F1-score de 0,91) e negativas (F1-score de 0,81, com Recall de 0,86).
- Comentários neutros (nota 3) são ambíguos e tiveram baixa previsibilidade (Recall de 6%).
- Recomendação de negócio: adotar um modelo de moderação híbrido, em que a IA faz a triagem dos extremos (elogios e reclamações graves) e as avaliações neutras seguem para análise humana.

## Estrutura do Projeto

```text
analise-sentimentos-ecommerce/
├── analise_avaliacoes_olist.ipynb
├── README.md
└── .gitignore
```
