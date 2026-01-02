# 📡 TelecomX - Análise de Churn (Evasão de Clientes)

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=GREEN&style=for-the-badge)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)

## 📄 Descrição do Projeto

Este projeto consiste em uma análise exploratória de dados (EDA) completa focada em identificar os perfis de clientes com maior probabilidade de abandonar a empresa (**Churn**).

O objetivo é transformar dados brutos em insights de negócio acionáveis, permitindo que a empresa **TelecomX** adote estratégias preventivas para reduzir a perda de receita.

---

## 🎯 Objetivos de Negócio
1.  Identificar os **principais fatores** que levam ao cancelamento.
2.  Traçar o **perfil de risco** do cliente.
3.  Propor um **Plano de Ação** baseado em dados para retenção.

---

## 🛠️ Tecnologias Utilizadas

* **Python 3.x**
* **Pandas:** Manipulação e limpeza de dados (ETL).
* **NumPy:** Cálculos matemáticos.
* **Matplotlib & Seaborn:** Visualização estática de dados.
* **Plotly:** Visualizações interativas (Sunburst, Treemaps).

---

## ⚙️ Processamento de Dados (ETL)

O projeto seguiu um pipeline rigoroso de tratamento de dados:
1.  **Extração:** Carregamento de dados em formato JSON aninhado e normalização.
2.  **Limpeza:** Tratamento de valores vazios em colunas críticas (`Churn`, `Charges.Total`) e conversão de tipos (objetos para numéricos).
3.  **Engenharia de Atributos:**
    * Transformação de variáveis binárias (Yes/No -> 1/0).
    * Cálculo de Custo Diário.

---

## 📊 Principais Insights

A análise revelou padrões claros de comportamento. Abaixo estão os destaques:

### 1. A "Zona de Perigo" (Tenure)
A maior taxa de evasão ocorre nos primeiros **6 meses** de contrato. Clientes que superam essa barreira tendem a permanecer longos períodos.

### 2. O Vilão dos Contratos
O contrato **Mensal (Month-to-month)** apresenta uma taxa de churn drasticamente superior aos contratos anuais, indicando baixa fidelidade neste segmento.

### 3. Fibra Ótica e Pagamento
* Clientes com internet de **Fibra Ótica** cancelam mais do que usuários de DSL, sugerindo problemas de custo-benefício ou qualidade técnica.
* O método de pagamento **"Electronic Check"** tem forte correlação com a evasão.

### 4. Perfil Demográfico
Cidadãos Idosos (**Senior Citizens**) possuem uma taxa de cancelamento proporcionalmente maior que a média da base.

---

## 💡 Plano de Ação Recomendado

Com base nos dados, sugerem-se as seguintes estratégias para a TelecomX:

| Problema Identificado | Ação Sugerida |
| :--- | :--- |
| **Evasão Inicial (0-6 meses)** | Criar programa de *Onboarding* intensivo e descontos progressivos nos primeiros 90 dias. |
| **Pagamento via Cheque Eletrônico** | Incentivar migração para Débito Automático com 5% de desconto (reduz atrito de pagamento). |
| **Alta Evasão em Fibra Ótica** | Realizar auditoria técnica na rede de fibra e revisar preços frente à concorrência. |
| **Público Idoso** | Criar canal de suporte técnico exclusivo e simplificado ("Tech Support Senior"). |

---

## 📂 Estrutura do Notebook

1.  **Extração e Carregamento:** Leitura do JSON.
2.  **Limpeza de Dados:** Tratamento de nulos e tipos.
3.  **Análise Exploratória (EDA):**
    * Análise Demográfica (Gênero, Idade).
    * Análise de Serviços (Internet, Telefone).
    * Análise Financeira (Gastos mensais e totais).
4.  **Conclusão:** Relatório executivo.
---
