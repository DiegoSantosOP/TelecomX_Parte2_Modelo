# 📈 Análise de Evasão de Clientes (Churn) - Telecom

## 📍 Sobre o Projeto

Este projeto de Data Science aprofunda a análise da evasão de clientes (*churn*) em uma empresa de telecomunicações. Utilizando uma abordagem completa que vai da análise exploratória de dados (EDA) até a construção de modelos preditivos robustos, o objetivo é identificar os principais fatores de risco e fornecer *insights* acionáveis para estratégias de retenção.

---

## 🎯 Objetivos

- **Compreender o Perfil:** Analisar a fundo o perfil dos clientes que cancelam para identificar padrões e variáveis-chave.
- **Construir Modelos:** Desenvolver e comparar modelos de *machine learning* para prever a probabilidade de *churn*.
- **Propor Estratégias:** Sugerir ações de negócio baseadas em evidências para reduzir a taxa de evasão.

---

## 📂 Dados Utilizados

O dataset inclui informações detalhadas sobre os clientes, cobrindo:

- **Dados Demográficos:** Gênero, idade (*Senior Citizen*), dependentes, parceiro.
- **Serviços Contratados:** Internet (*Fiber Optic*, *DSL*), telefone e serviços adicionais.
- **Informações de Contrato:** Tipo de contrato, forma de pagamento, e tempo de contrato (*tenure*).
- **Custos:** Cobranças mensais e totais.
- **Variável-Alvo (`churn`):** Indica se o cliente cancelou o serviço.

---

## ⚙️ Etapas Metodológicas

1.  **Pré-processamento:** Limpeza, padronização e codificação de variáveis categóricas (`One-Hot Encoding`).
2.  **Análise Exploratória:** Investigação de correlações e visualizações para identificar o desbalanceamento de classes e os primeiros preditores de *churn*.
3.  **Balanceamento de Classes:** Aplicação da técnica **SMOTE** no conjunto de treino para tratar o desequilíbrio e melhorar o desempenho dos modelos.
4.  **Modelagem Preditiva:** Treinamento e avaliação de três modelos: **Regressão Logística**, **Random Forest** e **KNN**.
5.  **Otimização:** Ajuste de hiperparâmetros com `GridSearchCV` para o modelo Random Forest.
6.  **Análise Crítica:** Avaliação detalhada do desempenho dos modelos e da importância das variáveis para cada algoritmo.

---

## 📊 Principais Insights e Descobertas

* **Fatores de Risco:** Clientes com **contrato mensal**, serviço de internet **`Fiber Optic`** e que usam **`Electronic Check`** são consistentemente identificados como os mais propensos à evasão.
* **Tempo e Custo:** **Tempo de contrato** baixo e **gastos totais** reduzidos são fortes indicadores de *churn*, enquanto clientes fiéis e de alto gasto são a base mais estável.
* **Desempenho dos Modelos:** A **Regressão Logística** obteve o melhor desempenho geral, com um **AUC de 0.84** e um **Recall de 0.80**, mostrando grande eficácia em identificar clientes em risco.

---

## 💡 Estratégias de Retenção Sugeridas

- **Fidelização:** Criar programas de incentivo para clientes de contrato mensal, visando convertê-los para planos de longa duração.
- **Campanhas Segmentadas:** Direcionar campanhas de retenção para clientes de fibra óptica e aqueles que utilizam cheque eletrônico, oferecendo suporte proativo ou benefícios exclusivos.
- **Uso do Modelo:** Integrar o modelo de **Regressão Logística** em sistemas de CRM para identificar clientes de alto risco em tempo real, permitindo a atuação proativa da equipe de retenção.

---

## 🛠 Tecnologias Utilizadas

* **Linguagem:** Python
* **Bibliotecas:** Pandas, NumPy, Scikit-learn, Imbalanced-learn, Seaborn, Matplotlib

---


## 👨‍💻 Autor

| [<img src="https://github.com/user-attachments/assets/b753da45-f62e-474e-9e98-f227bc0c0be5" width=115><br><sub>Diego Santos</sub>](https://github.com/DiegoSantosOP) |
| :---: |
