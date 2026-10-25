# Classificador Naive Bayes para Detecção de Spam

Este repositório contém a implementação prática de um classificador probabilístico para triagem automatizada de mensagens (Spam vs. Ham). O projeto utiliza a técnica de Processamento de Linguagem Natural (PLN) Bag of Words para vetorização de texto e o algoritmo Multinomial Naive Bayes para a classificação.

## Objetivo

Desenvolver um modelo preditivo capaz de distinguir mensagens legítimas (Ham) de mensagens fraudulentas (Spam). O projeto aborda conceitos fundamentais de engenharia de machine learning, como a prevenção de vazamento de dados (Data Leakage) e o uso de log-probabilidades para evitar underflow numérico.

## Tecnologias Utilizadas

- Python 3
- Scikit-Learn (CountVectorizer, MultinomialNB, Pipelines)
- Pandas (Manipulação de dados tabulares)
- Matplotlib (Visualização da matriz de confusão)
- Jupyter Notebook / VS Code
- UV (Gerenciamento de pacotes e ambiente virtual)

## Estrutura do Projeto

```text
am-naive-bayes-spam/
├── src/am_naive_bayes_spam/   # Código-fonte base do pacote
├── pratica_naive_bayes.ipynb  # Notebook principal com a análise e o modelo
├── pyproject.toml             # Definição de dependências do projeto
├── uv.lock                    # Versões travadas das dependências
└── README.md                  # Documentação do projeto

```



## Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/Leandro-dsm/am-naive-bayes-spam.git
   cd am-naive-bayes-spam
   ```

2. Sincronize o ambiente virtual e as dependências (utilizando o UV):
   ```bash
   uv sync
   ```

3. Abra o notebook:
   ```bash
   uv run jupyter notebook pratica_naive_bayes.ipynb
   ```
   *(Alternativamente, o arquivo pode ser aberto e executado diretamente pelo VS Code).*

## Resultados e Aprendizados

O modelo foi treinado e avaliado através de uma divisão estratificada (70% treino / 30% teste). A avaliação incluiu:
- Relatório de classificação (Acurácia, Precisão, Recall e F1-score).
- Matriz de Confusão para visualização dos falsos positivos e falsos negativos.
- Teste de inferência com novas mensagens em tempo real.
- Implementação de um Pipeline unificado para automatizar o fluxo de pré-processamento e predição.

## Autor

**Leandro Sueoka** - [Leandro-dsm](https://github.com/Leandro-dsm)
