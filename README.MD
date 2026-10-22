# Previsão de Score de Crédito de Clientes com Machine Learning

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![Scikit--learn](https://img.shields.io/badge/Scikit--learn-Machine%20Learning-F7931E?logo=scikit-learn&logoColor=white)

## Descrição

Modelo de Machine Learning que prevê o **score de crédito** de clientes de um banco, classificando-os em **Ruim, Ok ou Bom**, a partir de uma base com **100.000 clientes**.

Esse tipo de modelo é usado por instituições financeiras para apoiar decisões de concessão de crédito, definição de limites e análise de risco de inadimplência.

---

## Resultados

| Modelo | Acurácia |
|---|---|
| **Random Forest** ✅ | **82,6%** |
| KNN | 73,5% |

O **Random Forest** foi o modelo escolhido, acertando o score em mais de 8 a cada 10 clientes.

---

## Tecnologias

Python · Pandas · Scikit-learn · Jupyter Notebook

---

## Etapas do projeto

1. **Importação da base** — carregamento dos dados dos clientes
2. **Análise inicial** — tipos de variáveis, dados ausentes
3. **Tratamento dos dados** — codificação de variáveis categóricas (`profissao`, `mix_credito`, `comportamento_pagamento`) com `LabelEncoder`
4. **Treinamento** — comparação entre Random Forest e KNN
5. **Avaliação** — escolha do melhor modelo por acurácia
6. **Previsão** — aplicação do modelo em novos clientes

---

## Como executar

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
pip install pandas scikit-learn jupyter
jupyter notebook
```

Abra o `.ipynb` e execute as células em ordem (`clientes.csv` e `novos_clientes.csv` devem estar na mesma pasta).


Feito por Giovanna Dantas.
