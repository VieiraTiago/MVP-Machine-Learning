# MVP: Machine Learning & Analytics

**Autor:** Tiago Santos Vieira  
**Data:** 18/09/2025  
**Matrícula:** 4052023000279

Este projeto tem como objetivo desenvolver um modelo preditivo capaz de identificar o risco jurídico de empresas do setor energético com base em variáveis financeiras, operacionais e institucionais. A solução foi construída com foco em robustez, interpretabilidade e aplicabilidade prática em contextos de auditoria, compliance e gestão de risco.

---

## Estrutura do Projeto

- `Notebook_Engenharia_de_Dados.ipynb`: Notebook principal com todas as etapas do projeto, incluindo EDA, preparação de dados, modelagem e avaliação.
- `data/`: Pasta destinada ao armazenamento do dataset (não incluído por questões de privacidade).
- `README.md`: Documento explicativo do projeto.

---

## Objetivo

Classificar empresas quanto ao risco de envolvimento em litígios, utilizando dados tabulares estruturados. A tarefa é tratada como um problema de **classificação binária**, com foco em antecipação de riscos jurídicos e suporte à tomada de decisão.

---

## Técnicas Utilizadas

- Análise exploratória de dados (EDA)
- Engenharia de atributos
- Pipelines com `scikit-learn`
- Validação cruzada com `KFold`
- Modelos supervisionados:
  - `DummyClassifier` (baseline)
  - `RandomForestClassifier`
  - `LogisticRegression`
  - Rede Neural com `Keras`
- Métricas de avaliação: acurácia, F1-score, matriz de confusão, classification report

---

## Principais Achados

- O modelo **Random Forest** apresentou acurácia média de **0.80**, superando a baseline de **0.74**
- A **Regressão Logística** teve desempenho competitivo com maior interpretabilidade
- A variável derivada `Revenue_per_Employee` mostrou forte poder discriminativo
- A distribuição da variável-alvo revelou **desbalanceamento**, tratado com `class_weight='balanced'`
- A rede neural apresentou desempenho promissor, mas com maior custo computacional

---

## 🛠Requisitos

- Python 3.12+
- Bibliotecas:
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`
  - `scikit-learn`
  - `keras`

---

## Como Executar

1. Clone o repositório:
   ```bash
   git clone https://github.com/VieiraTiago/MVP-Machine-Learning.git
