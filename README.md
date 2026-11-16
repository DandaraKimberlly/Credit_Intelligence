<div align="center">

# 💳 Credit Intelligence Analytics

**Investigação de padrões de risco de inadimplência em cartões de crédito com fluxo analítico de ponta a ponta (*end-to-end*).**

![Status](https://img.shields.io/badge/Status-Em%20Desenvolvimento-yellow?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)

*Projeto de análise de dados utilizando Python, SQL, PostgreSQL, Power BI e Machine Learning.*

</div>

---

## 📋 Índice

- [1. O Projeto](#-1-o-projeto)
- [2. Problema de Negócio](#-2-problema-de-negócio)
- [3. Objetivos](#-3-objetivos)
- [4. Base de Dados](#-4-base-de-dados)
- [5. Tecnologias e Ferramentas](#-5-tecnologias-e-ferramentas)
- [6. Estrutura do Projeto](#-6-estrutura-do-projeto)
- [7. Etapas de Desenvolvimento](#-7-etapas-de-desenvolvimento)
- [8. Fonte e Atribuição](#-8-fonte-e-atribuição)

---

## 🎯 1. O Projeto

O **Credit Intelligence** busca demonstrar como os dados podem apoiar análises de risco de crédito e decisões de negócio.

A proposta é desenvolver um fluxo analítico de ponta a ponta (*end-to-end*), passando pela obtenção, armazenamento, validação, exploração e transformação dos dados, até a construção de indicadores, visualizações e um modelo preditivo experimental.

> 💡 O projeto combina conhecimentos de **Engenharia de Dados**, **Análise de Dados** e **Machine Learning**.

---

## 🔍 2. Problema de Negócio

A avaliação do risco de crédito envolve compreender o comportamento de pagamento dos clientes e identificar padrões que possam estar associados à inadimplência.

A partir de uma base histórica de clientes de cartão de crédito, investiguei questões como:

- 📊 Qual é a distribuição e o perfil de clientes que apresentaram inadimplência?
- 🔄 Quais padrões de pagamento aparecem com maior frequência entre os clientes inadimplentes?
- 💰 Como o limite de crédito e os valores das faturas se relacionam com o comportamento de pagamento?
- 📈 Quais indicadores podem apoiar a compreensão do risco de crédito?

---

## 🚀 3. Objetivos

- [ ] Estruturar e validar uma base de dados relacional.
- [ ] Aplicar consultas SQL para investigação e extração de informações.
- [ ] Realizar análise exploratória de dados (EDA).
- [ ] Identificar padrões, distribuições e possíveis inconsistências.
- [ ] Desenvolver indicadores de negócio relacionados ao risco de crédito.
- [ ] Aplicar técnicas de preparação de variáveis (*feature engineering*).
- [ ] Desenvolver e avaliar modelos experimentais de classificação.
- [ ] Construir um dashboard interativo para comunicar os principais resultados.

---

## 🗄️ 4. Base de Dados

* **Dataset:** Default of Credit Card Clients
* **Fonte:** UCI Machine Learning Repository
* **Link de Acesso:** [UCI Repository - Default of Credit Card Clients](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients)

### Características informadas pela fonte:
* **Volume:** 30.000 registros de clientes.
* **Atributos:** 23 variáveis explicativas.
* **Origem:** Dados históricos de clientes de cartão de crédito de Taiwan.
* **Período:** Histórico de pagamentos de abril a setembro de 2005.
* **Alvo:** Variável-alvo relacionada à inadimplência no mês seguinte.

### Variável-alvo (`default.payment.next.month`)
| Valor | Significado |
| :---: | :--- |
| **`0`** | Não houve inadimplência no mês seguinte |
| **`1`** | Houve inadimplência no mês seguinte |

---

## 🛠️ 5. Tecnologias e Ferramentas

| Tecnologia / Ferramenta | Aplicação no Projeto |
| :--- | :--- |
| **Python** | Manipulação, análise e modelagem dos dados |
| **Pandas e NumPy** | Tratamento e operações com dados |
| **Matplotlib e Seaborn** | Visualização e análise exploratória |
| **Scikit-learn** | Desenvolvimento e avaliação de modelos |
| **PostgreSQL** | Armazenamento e gerenciamento dos dados |
| **SQL** | Consultas, validações e indicadores |
| **DBeaver** | Administração visual do banco de dados |
| **Power BI** | Construção do dashboard |
| **Jupyter Notebook** | Desenvolvimento e documentação das análises |
| **Git e GitHub** | Versionamento e compartilhamento do projeto |

---

## 📂 6. Estrutura do Projeto

```text
credit-intelligence-analytics/
│
├── 1_dados/                 # Armazenamento dos arquivos de dados
│   ├── originais/           # Dados brutos extraídos da fonte
│   └── tratados/            # Dados limpos e prontos para análise
│
├── 2_notebooks/             # Jupyter Notebooks com EDA, feature engineering e ML
├── 3_sql/                   # Scripts de criação de tabelas, consultas e indicadores
├── 4_src/                   # Códigos-fonte e módulos reutilizáveis em Python
├── 5_dashboard/             # Arquivos do Power BI (.pbix)
│   └── screenshots/         # Capturas de tela do dashboard para documentação
├── 6_relatorios/            # Documentos e relatórios de resultados
├── 7_imagens/               # Gráficos exportados e recursos visuais
│
├── .gitignore               # Arquivos ignorados pelo controle de versão
├── environment.yml          # Configuração das dependências do ambiente Python
├── LICENSE                  # Licença do projeto
└── README.md                # Documentação principal

## 🗺️ 7. ETAPAS PARA DESENVOLVIMENTO DO PROJETO

**Fase 1 — Estruturação do projeto**
- Organização dos diretórios.
- Configuração do ambiente Python.
- Preparação do repositório GitHub.
- Documentação inicial.

**Fase 2 — Engenharia de Dados**
- Configuração do PostgreSQL e DBeaver.
- Modelagem e criação das tabelas.
- Importação e validação dos dados.
- Consultas SQL e análise da qualidade dos dados.

**Fase 3 — Análise Exploratória de Dados**
- Análise estatística e descritiva.
- Investigação de distribuições e relações entre variáveis.
- Identificação de padrões associados à inadimplência.

**Fase 4 — Engenharia de Atributos**
- Preparação das variáveis.
- Transformações e seleção de atributos.
- Preparação dos dados para modelagem.

**Fase 5 — Modelagem Preditiva**
- Treinamento de modelos de classificação.
- Avaliação de desempenho.
- Análise de métricas e limitações.

**Fase 6 — Business Intelligence**
- Construção de indicadores.
- Desenvolvimento do dashboard no Power BI.
- Comunicação dos principais resultados.

## 📚 8. FONTE E ATRIBUIÇÃO

Yeh, I. (2009). *Default of Credit Card Clients* [Dataset]. UCI Machine Learning Repository.

DOI: https://doi.org/10.24432/C55S3H

Licença da base de dados: Creative Commons Attribution 4.0 International (CC BY 4.0).

A fonte será devidamente atribuída e eventuais alterações realizadas na base serão documentadas.

---

Construído para fins de aprendizado, aplicação prática de conhecimentos em Analytics e demonstração de competências em Engenharia e Análise de Dados.