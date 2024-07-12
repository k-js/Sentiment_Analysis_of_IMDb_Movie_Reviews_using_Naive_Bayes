# Análise de Sentimentos em Avaliações de Filmes usando Naive Bayes

## Descrição

Este projeto utiliza o algoritmo Naive Bayes para realizar análise de sentimentos em avaliações de filmes do conjunto de dados IMDb Movie Reviews. O objetivo é classificar se uma avaliação é positiva ou negativa com base no texto da revisão.

## Motivação

A análise de sentimentos em avaliações de filmes é uma aplicação comum de técnicas de aprendizado de máquina na indústria de entretenimento e serviços de streaming. Este projeto serve como uma introdução prática ao uso do Naive Bayes para classificação de textos.

## Conjunto de Dados

O conjunto de dados utilizado é o IMDb Movie Reviews Large Dataset, disponível no Kaggle. Ele contém avaliações de filmes rotuladas como positivas ou negativas.

## Funcionalidades

- **Pré-processamento de Texto:** Utiliza `CountVectorizer` do `scikit-learn` para vetorizar as avaliações de filmes.
- **Modelo Naive Bayes:** Implementa um classificador `MultinomialNB` para treinar e prever sentimentos das avaliações.
- **Avaliação de Desempenho:** Calcula a acurácia do modelo na classificação de avaliações como positivas ou negativas.

## Requisitos

- Python 3.x
- Bibliotecas Python: `numpy`, `pandas`, `scikit-learn`

## Como Executar

1. Clone o repositório:

git clone https://github.com/seu-usuario/analisador-sentimentos-filmes.git
cd analisador-sentimentos-filmes

2. Instale as dependências:
   
pip install -r requirements.txt


3. Execute o notebook Jupyter:

jupyter notebook


Abra o notebook `Analisador_Sentimentos_Filmes.ipynb` e execute todas as células.

## Exemplo de Uso

Após treinar o modelo, você pode inserir novas avaliações de filmes para classificação de sentimentos. Por exemplo:

```python
# Exemplo de classificação de uma nova avaliação
new_review = ["This movie was great, I loved it!"]
new_review_vectorized = vectorizer.transform(new_review)
prediction = model.predict(new_review_vectorized)
print(f'Classificação da nova avaliação: {"Positive" if prediction[0] == 1 else "Negative"}')


Este README.md utiliza as tags do Markdown para estruturar e formatar as seções do projeto de análise de sentimentos em avaliações de filmes usando Naive Bayes. Lembre-se de personalizar com informações específicas do seu projeto, como links para o conjunto de dados utilizado, instruções detalhadas de instalação e execução, e detalhes adicionais sobre a implementação do modelo.



