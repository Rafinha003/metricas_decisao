# 📊 Métricas Tradicionais vs Modelos de Decisão

Este repositório demonstra, de forma **simples e didática**, por que métricas tradicionais de Machine Learning (como **acurácia, F1-score ou RMSE**) podem falhar quando usadas para **modelos de decisão**, mesmo apresentando ótimos resultados técnicos.

O objetivo é mostrar que **prever bem não é o mesmo que decidir bem**.

---

## 🎯 Motivação

Em muitos problemas reais de Data Science, o modelo não é usado apenas para prever um evento, mas para **orientar uma ação de negócio**.

Exemplos comuns:

* Oferecer ou não um desconto
* Entrar ou não em contato com um cliente
* Aprovar ou não um crédito

Métricas tradicionais avaliam **qualidade da previsão**, mas não medem o **impacto da decisão tomada a partir dessa previsão**.

---

## 🤖 Modelo Preditivo vs Modelo de Decisão

### 🔹 Modelo preditivo

Responde perguntas como:

> "Qual a probabilidade de um cliente cancelar?"

Métricas comuns:

* Acurácia
* F1-score
* RMSE

### 🔹 Modelo de decisão

Responde perguntas como:

> "O que acontece se eu oferecer um desconto a este cliente?"

Aqui, o interesse está no **efeito da ação**, e não apenas na previsão do evento.

---

## 🧪 O Experimento

Neste projeto, foi criado um **dataset sintético** simulando um problema de **churn**, contendo:

* `uso_produto`: intensidade de uso do cliente
* `reclamacoes`: número de reclamações
* `desconto_oferecido`: ação controlável pelo negócio

No mundo simulado:

* O desconto **realmente reduz churn**
* Mas essa informação **não é corretamente avaliada apenas pela acurácia**

Um modelo de **Regressão Logística** é treinado e avaliado usando métricas tradicionais.

---

## 📉 Resultado Principal

Mesmo com **alta acurácia**, o modelo:

* Não consegue responder perguntas contrafactuais
* Não mede o impacto real da ação
* Pode sugerir decisões que não geram valor

Ou seja:

> **Boa métrica ≠ boa decisão**

---


## 📂 Estrutura do Repositório

```
metricas_decisao/
│
├── notebook.ipynb   # Notebook com experimento e explicações
├── README.md        # Este arquivo
```

---

## 🚀 Objetivo do Projeto

Este projeto foi criado com foco em:

* Aprendizado prático
* Clareza conceitual
* Discussões sobre métricas, impacto e decisão




Se esse conteúdo te ajudou ou gerou alguma reflexão, fique à vontade para abrir uma issue ou trocar ideia no LinkedIn 🚀
