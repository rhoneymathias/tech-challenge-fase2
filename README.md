# 🍷 Classificação da Qualidade de Vinhos utilizando Machine Learning

## 📖 Sobre o Projeto

Este projeto foi desenvolvido como parte do **Tech Challenge – Fase 2** da **Pós-Tech em Data Analytics da FIAP**.

O objetivo consiste em desenvolver e comparar modelos de **Machine Learning** capazes de prever se um vinho será classificado como de **alta qualidade** antes da avaliação sensorial, utilizando apenas características físico-químicas obtidas em laboratório.

A proposta busca demonstrar como técnicas de Inteligência Artificial podem auxiliar o processo decisório da indústria vitivinícola, reduzindo a subjetividade da avaliação humana e fornecendo uma ferramenta de apoio ao controle de qualidade durante a produção.

---

## 🎯 Problema de Negócio

A avaliação da qualidade do vinho é tradicionalmente realizada por especialistas por meio de análises sensoriais. Apesar de essencial, esse processo demanda tempo, experiência e apresenta elevado grau de subjetividade.

Diante desse cenário, este projeto busca responder à seguinte questão:

> **É possível prever, por meio das características físico-químicas do vinho, se um produto será classificado como de alta qualidade antes mesmo da avaliação sensorial?**

Para responder essa pergunta, foram desenvolvidos modelos de classificação supervisionada capazes de identificar vinhos de **alta qualidade (quality ≥ 7)** e **baixa/média qualidade (quality < 7)**.

---

## 📊 Base de Dados

Foi utilizada a base pública **WineQT**, composta por:

- 1.143 amostras de vinhos;
- 11 variáveis físico-químicas;
- 1 variável alvo (quality).

As principais variáveis analisadas são:

- Fixed Acidity
- Volatile Acidity
- Citric Acid
- Residual Sugar
- Chlorides
- Free Sulfur Dioxide
- Total Sulfur Dioxide
- Density
- pH
- Sulphates
- Alcohol

---

## 🔍 Etapas Desenvolvidas

O projeto foi desenvolvido seguindo as principais etapas de um fluxo de Machine Learning:

- Análise exploratória dos dados (EDA);
- Verificação de valores ausentes e duplicados;
- Análise da distribuição da variável alvo;
- Estudo da correlação entre as variáveis;
- Transformação da variável de qualidade em classificação binária;
- Divisão dos dados em treino e teste;
- Padronização das variáveis utilizando StandardScaler;
- Treinamento e comparação dos modelos de classificação;
- Avaliação e interpretação dos resultados.

---

## 🤖 Modelos Utilizados

Foram avaliados os seguintes algoritmos de Machine Learning:

- Regressão Logística
- Random Forest

Os modelos foram comparados utilizando métricas de desempenho, sendo selecionado aquele com maior capacidade de generalização.

---

## 📈 Principais Resultados

Os resultados demonstraram que as características físico-químicas permitem prever a qualidade do vinho com elevado grau de confiabilidade.

Entre os modelos avaliados, o **Random Forest** apresentou o melhor desempenho, alcançando aproximadamente **85% de acurácia**, sendo selecionado como o modelo mais adequado para o problema proposto.

### Resultados Obtidos

| Modelo | Acurácia | Observação |
|---------|:--------:|------------|
| Regressão Logística | 76,97% | Desempenho satisfatório, porém inferior ao Random Forest. |
| **Random Forest** | **85,42%** | Melhor desempenho entre os modelos avaliados. |

Além da elevada capacidade preditiva, o modelo Random Forest identificou as variáveis físico-químicas mais relevantes para a classificação da qualidade dos vinhos:

- 🍷 Teor alcoólico (Alcohol)
- 🍷 Acidez volátil (Volatile Acidity)
- 🍷 Sulfatos (Sulphates)
- 🍷 Ácido cítrico (Citric Acid)

Esses resultados demonstram o potencial da aplicação de técnicas de Machine Learning como ferramenta de apoio à tomada de decisão na indústria vitivinícola, permitindo identificar antecipadamente vinhos com maior probabilidade de atingir elevados padrões de qualidade.
---

## 🛠️ Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- GitHub
