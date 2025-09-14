# Pipeline de Dados Públicos com AWS Glue

Este repositório contém um pipeline de dados construído na **AWS** para realizar processos de **ETL** (Extract, Transform, Load) em dados públicos.  
O projeto demonstra boas práticas no uso de serviços serverless como **S3**, **Glue**, **Athena** e **QuickSight**.

---

## 📚 Descrição do Projeto

O pipeline realiza:

- **Coleta de dados públicos** em formato CSV/JSON.
- **Armazenamento bruto** no Amazon S3 (data lake).
- **Transformação** com scripts em PySpark no AWS Glue (limpeza, normalização, enriquecimento).
- **Carga dos dados tratados** em formato otimizado (Parquet) em um bucket estruturado.
- **Catalogação** no Glue Data Catalog para consultas rápidas.
- **Consumo dos dados** via Amazon Athena e visualizações no QuickSight.

---

## 🗂 Estrutura do Repositório

pipeline-dados-publicos-aws-glue/
│
├── README.md # Documentação do projeto
├── docs/ # Documentos e diagramas
│ └── diagrama_pipeline.png
├── data/ # Exemplos de dados públicos
│ └── exemplo_dados.csv
└── scripts/ # Códigos do pipeline
├── glue_jobs/ # Jobs do AWS Glue em PySpark
│ └── job_etl.py
└── tests/ # Scripts de teste/validação


---

## 🛠 Pré-requisitos

- Conta AWS ativa.
- Permissões para usar:
  - Amazon S3
  - AWS Glue
  - AWS Athena
  - (opcional) Amazon QuickSight para dashboards
- Python 3.x (para scripts locais ou testes).

---

## 🚀 Como Executar

1. **Clone o repositório:**
   ```bash
   git clone https://github.com/seu-usuario/pipeline-dados-publicos-aws-glue.git
   cd pipeline-dados-publicos-aws-glue
aws configure
