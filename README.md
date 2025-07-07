# 📧 Classificador de Spam com Machine Learning

Este projeto utiliza aprendizado de máquina para **classificar mensagens como spam ou não-spam** com base no conteúdo textual.

📂 Tecnologias usadas:
- Python
- Pandas, Numpy
- Scikit-learn (Tfidf, Naive Bayes)
- Matplotlib e Seaborn para visualizações

---

## 📌 Objetivo do Projeto

Desenvolver um classificador de spam simples usando:
- **TF-IDF** para transformar texto em vetores numéricos
- **Multinomial Naive Bayes** como modelo de aprendizado
- **Avaliação com acurácia, matriz de confusão e relatório de classificação**

---

## 🚀 Pipeline do Projeto

Abaixo está o **fluxo completo** do projeto em etapas:

### 1. Importação das bibliotecas

![Etapa 1](importar-bibliotecas.png)

---

### 2. Leitura e pré-processamento do dataset

![Etapa 2](carregar-dataset.png)

- Dataset `spam.csv` contendo mensagens rotuladas como `spam` ou `ham`.
- Renomeamos as colunas e transformamos os rótulos para 0 (ham) e 1 (spam).

---

### 3. Separação de treino e teste

![Etapa 3](assets/etapa3-train-test.png)

- Utilizamos `train_test_split` com 20% para teste.
- Mantemos a distribuição com `random_state=42` para reprodutibilidade.

---

### 4. Vetorização com TF-IDF

![Etapa 4](assets/etapa4-tfidf.png)

- Treinamos o vetorizador **apenas nos dados de treino** (`fit_transform`)
- Depois transformamos os dados de teste com o mesmo vocabulário (`transform`)

---

### 5. Treinamento do modelo

![Etapa 5](assets/etapa5-modelo.png)

- Utilizamos `MultinomialNB`, modelo leve e eficaz para texto.

---

### 6. Avaliação do modelo

![Etapa 6](assets/etapa6-avaliacao.png)

- Acurácia superior a 95%
- Matriz de confusão para análise dos erros
- Classificação detalhada com precisão, recall e f1-score

---

## 🧠 Mapa Mental

Criei um mapa mental resumindo as bibliotecas utilizadas:

![Mapa Mental](assets/mapa-mental-classificador-spam.png)

---

## 🔗 Executar no Google Colab

Se quiser testar o projeto, abra o notebook no Colab:

👉 [Abrir no Colab](https://colab.research.google.com/drive/SEU_LINK_AQUI)

---

## 📬 Contato

Caso tenha interesse em discutir ou melhorar o projeto:

📧 SeuNomeDev@gmail.com  
💼 [linkedin.com/in/seunome](https://linkedin.com/in/seunome)

---

## ✅ Status

✔️ Projeto funcional e didático  
🔜 Próximo passo: adicionar limpeza de texto (stopwords, stemming)

