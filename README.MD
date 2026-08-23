# Previsão de Score de Crédito de Clientes com Machine Learning

## Descrição
Este projeto tem como objetivo construir um **modelo de Machine Learning capaz de prever o score de crédito de clientes de um banco**.

A partir de uma base de dados contendo informações sobre **100.000 clientes**, foram realizadas etapas de **tratamento de dados, análise exploratória e treinamento de modelos de classificação**, com o objetivo de classificar cada cliente em uma das três categorias de score: **Ruim, Ok ou Bom**.

Esse tipo de modelo é extremamente importante para instituições financeiras, pois auxilia na tomada de decisões relacionadas a:
- concessão de crédito
- empréstimos
- definição de limites
- análise de risco de inadimplência

---

## Tecnologias utilizadas
- Python
- Pandas
- Scikit-learn
- Jupyter Notebook

---

## Objetivo do projeto
Criar um modelo capaz de classificar o score de crédito de um cliente em **Ruim, Ok ou Bom**, utilizando algoritmos de **Machine Learning supervisionado**.

---

## Etapas do projeto

O projeto foi desenvolvido seguindo as seguintes etapas:

### 1. Importação da base de dados
Carregamento da base contendo informações dos clientes.

---

### 2. Análise inicial dos dados
- Verificação de dados ausentes
- Identificação de tipos de variáveis
- Inspeção geral da base de dados

---

### 3. Tratamento dos dados
- Codificação de variáveis categóricas (profissão, mix de crédito e comportamento de pagamento) com `LabelEncoder`
- Preparação da base para o treinamento dos modelos

---

### 4. Seleção das variáveis
Definição das colunas que serão utilizadas como **features** (variável `x`) e da coluna alvo `score_credito` (variável `y`) para o modelo de Machine Learning.

---

### 5. Treinamento dos modelos
Foram utilizados dois algoritmos de classificação:
- **Random Forest** (`RandomForestClassifier`)
- **KNN — K-Nearest Neighbors** (`KNeighborsClassifier`)

Esses modelos foram treinados para prever o **score de crédito dos clientes** (Ruim, Ok ou Bom).

---

### 6. Avaliação dos modelos
Após o treinamento, os modelos foram avaliados por meio da métrica de **acurácia**, comparando as previsões com os dados de teste. O modelo **Random Forest** apresentou o melhor desempenho (aproximadamente 82,6% de acurácia, contra 73,5% do KNN) e foi escolhido para gerar as previsões finais.

---

### 7. Previsão de novos clientes
Com o modelo de melhor desempenho já treinado, o mesmo processo de codificação das variáveis categóricas foi aplicado a uma nova base de clientes, permitindo prever o score de crédito de novos casos.

---

## Importância do projeto
Projetos como este são amplamente utilizados no setor financeiro para:
- análise de risco de crédito
- prevenção de inadimplência
- definição de limites de crédito
- apoio à tomada de decisão
