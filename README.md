# Classificação de Sentimentos com spaCy 😄

Este repositório contém um tutorial completo sobre como construir um classificador de sentimentos usando a biblioteca spaCy em Python.  O objetivo é classificar textos como expressando "alegria" ou "medo".  Vamos passo a passo, desde a preparação dos dados até a avaliação do modelo.  Prepare-se para uma jornada divertida e informativa! 🚀

## 1. Introdução 👋

A análise de sentimentos é uma tarefa importante em processamento de linguagem natural (PLN).  Este tutorial demonstra como utilizar o spaCy, uma biblioteca poderosa e eficiente de PLN, para construir um classificador binário (alegria/medo).  Usaremos uma base de dados de exemplos de textos e suas respectivas emoções.

## 2. Pré-requisitos 🛠️

* **Python:** Certifique-se de ter o Python instalado na sua máquina.
* **Bibliotecas:** Precisaremos das seguintes bibliotecas:
    * `spacy`: Para processamento de linguagem natural.
    * `pandas`: Para manipulação de dados.
    * `scikit-learn`: Para métricas de avaliação (opcional, mas recomendado).
    * `seaborn`: Para visualização de dados (opcional, mas recomendado).
    * `matplotlib`: Para visualização de dados (opcional, mas recomendado).
* **Modelo de Linguagem:** Você precisará baixar o modelo de linguagem do spaCy para português: `pt_core_news_sm`.  Isso pode ser feito usando o comando `python -m spacy download pt_core_news_sm` no seu terminal.

## 3. Dados 🗂️

Este projeto utiliza duas bases de dados:

* `base_treinamento.txt`: Contém os dados para treinar o modelo.  Cada linha contém um texto e a emoção correspondente (alegria ou medo).
* `base_teste.txt`: Contém os dados para testar o modelo treinado.  Similar ao arquivo de treinamento, mas independente.


## 4. Etapas do Processo 👣

O código Python (`classificação_de_textos_com_spacy.py`) realiza as seguintes etapas:

1. **Importação de Bibliotecas:** Importa as bibliotecas necessárias para o projeto.
2. **Carregamento dos Dados:** Lê as bases de dados `base_treinamento.txt` e `base_teste.txt` usando o pandas.
3. **Pré-processamento:** Aplica pré-processamento aos textos, incluindo:
    * Conversão para minúsculas.
    * Lematização (redução das palavras à sua forma base).
    * Remoção de stop words (palavras comuns como "a", "o", "em").
    * Remoção de pontuação.
4. **Preparação dos Dados para o spaCy:** Transforma os dados em um formato adequado para o treinamento do modelo do spaCy.
5. **Treinamento do Modelo:** Treina um modelo de classificação de texto usando o spaCy.  O treinamento envolve iterações (épocas) sobre os dados de treinamento, ajustando os pesos do modelo para minimizar o erro.  O progresso do treinamento é monitorado e plotado.
6. **Salvar o Modelo:** Salva o modelo treinado em disco para uso posterior.
7. **Testes:** Testa o modelo com frases de exemplo para verificar seu funcionamento.
8. **Avaliação:** Avalia o desempenho do modelo usando métricas como acurácia e matriz de confusão, tanto na base de treinamento quanto na base de teste.

## 5. Como Executar 🚀

1. **Clone o repositório:** Clone este repositório para sua máquina local.
2. **Instale as bibliotecas:** Instale as bibliotecas listadas na seção de pré-requisitos usando `pip install -r requirements.txt` (crie um arquivo requirements.txt com as bibliotecas necessárias).
3. **Baixe o modelo de linguagem:** Execute `python -m spacy download pt_core_news_sm`.
4. **Execute o script:** Execute o script Python `classificação_de_textos_com_spacy.py`.

## 6. Resultados 📊

Os resultados do treinamento e da avaliação do modelo serão apresentados no console e em gráficos, mostrando a acurácia e a matriz de confusão para ambos os conjuntos de dados (treinamento e teste).  Isso permitirá avaliar a performance do classificador de sentimentos.

## 7. Contribuições 🤝

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

Espero que este tutorial ajude você a aprender como construir um classificador de sentimentos com spaCy!  Feliz codificação! 🎉
