# 🚀 Data Engineering & Big Data Cloud - Journey & Portfolio

Bem-vindo ao repositório central de estudos, projetos práticos e laboratórios desenvolvidos ao longo do **Roadmap de Especialização em Engenharia de Dados & Big Data Cloud**.

Este repositório está estruturado em **5 Fases Progressivas**, cobrindo desde os fundamentos em Python e SQL Analítico até arquiteturas distribuídas com **Apache Spark / Databricks**, **Delta Lake (Medallion)**, **Cloud (Azure)**, **Data Quality** e **CI/CD**.

---

## 📌 Estrutura do Repositório

```text
.
├── 📂 fase-1-fundamentos/          # Python Avançado, POO, SQL Analítico & Boas Práticas
├── 📂 fase-2-pyspark-spark/        # Apache Spark, PySpark, Spark UI & Performance Tuning
├── 📂 fase-3-databricks-delta/     # Databricks, Delta Lake & Arquitetura Medallion
├── 📂 fase-4-azure-cloud/          # Azure Data Platform (ADLS Gen2, ADF, Key Vault, FinOps)
├── 📂 fase-5-cicd-data-quality/    # GitHub Actions, pytest, Delta Expectations & Unity Catalog
└── 📂 projeto-integrador-final/    # 🏆 Projeto Capstone End-to-End em Databricks
```

---

## 🎯 Detalhamento por Fase e Projetos Práticos

### 🔹 Fase 1: Fundamentos Técnicos & Engenharia de Software

- **Foco:** Python Avançado (POO, typing, exceções), SQL Analítico (Window Functions, CTEs) e qualidade de código com `pytest` e `ruff`.
- **🛠️ Mini-Projeto:** Ingestor e Limpador de Arquivos Semi-Estruturados em Python com validação de schemas e exportação otimizada em Parquet.

### 🔹 Fase 2: Processamento Distribuído com PySpark & Spark Engine

- **Foco:** Arquitetura do Spark (Driver, Executors, DAG), PySpark DataFrames/SQL, e técnicas avançadas de otimização no Spark UI.
- **🛠️ Mini-Projeto / Estudo de Caso:** Diagnóstico e otimização de um pipeline com **Data Skew** e _Small Files Problem_, utilizando **Salting**, **Broadcast Joins** e **Adaptive Query Execution (AQE)**.

### 🔹 Fase 3: Databricks & Delta Lake (Arquitetura Medallion)

- **Foco:** Plataforma Databricks, Workspaces, Jobs, e gestão de tabelas ACID com Delta Lake.
- **🛠️ Mini-Projeto:** Construção de pipeline ETL em camadas (**Bronze**, **Silver** e **Gold**) utilizando `MERGE INTO` (Upserts), _Schema Enforcement_ e comandos `OPTIMIZE / VACUUM`.

### 🔹 Fase 4: Arquitetura Cloud (Azure Data Platform) & FinOps

- **Foco:** Armazenamento distribuído com Azure Data Lake Storage Gen2 (ADLS), gestão de segredos com Azure Key Vault e automação com Azure Data Factory.
- **🛠️ Mini-Projeto:** Conexão segura entre Azure Databricks e ADLS Gen2 via Service Principal / Managed Identity, aplicando estratégias de contenção de custos (FinOps).

### 🔹 Fase 5: CI/CD, Data Quality & Governança

- **Foco:** Automação de deploys, testes automatizados para pipelines de dados e catálogo/governança.
- **🛠️ Mini-Projeto:** Esteira de CI/CD via GitHub Actions para execução automatizada de linters e testes unitários com `pytest`, promovendo código para o Databricks via **Databricks Asset Bundles (DABs)**.

---

## 🏆 Projeto Integrador Final (Capstone)

**Tema:** _End-to-End Analytics & Predictive Feature Pipeline no Azure Databricks_

Um projeto completo reunindo todas as tecnologias estudadas:

1. **Ingestão (Bronze):** Captura automatizada de dados brutos e salvamento no ADLS Gen2.
2. **Transformação & Qualidade (Silver):** Limpeza, desduplicação e checagem de regras de qualidade (_Dead-Letter Queue_ / Quarentena).
3. **Agregação & Modelagem (Gold):** Modelagem multidimensional em Delta Lake pronta para consumo por BI e modelos de Machine Learning.
4. **CI/CD & Observabilidade:** Pipeline implantado via esteira de CI/CD com alertas de performance e orçamento no ambiente Cloud.

---

## 🛠️ Tecnologias & Ferramentas Utilizadas

- **Linguagens:** Python 3.x, SQL, PySpark
- **Engine & Processamento:** Apache Spark, Databricks, Delta Lake
- **Nuvem:** Azure (ADLS Gen2, Data Factory, Key Vault)
- **Engenharia de Software:** Git, GitHub Actions, `pytest`, `ruff`, Databricks CLI / DABs
- **Práticas:** Arquitetura Medallion, Data Quality, FinOps, CI/CD

---

## 💻 Como Utilizar / Executar os Projetos

1. **Clonar o Repositório:**
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio-dados.git
   cd seu-repositorio-dados
   ```
2. **Configurar o Ambiente Virtual Python:**
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Linux/Mac ou .venv\Scripts\activate no Windows
   pip install -r requirements.txt
   ```
3. **Executar Testes Unitários:**
   ```bash
   pytest
   ```

---

## 📝 Autor & Licença

Desenvolvido como repositório de evolução contínua em Engenharia de Dados.  
Licença: MIT.
