# ☁️ Projeto de Migração para Nuvem AWS - Farmácia Abstergo

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?style=for-the-badge&logo=amazon-aws)
![Status](https://img.shields.io/badge/Status-Concluído-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)

## 📋 Descrição do Projeto

Este projeto documenta a estratégia de migração e modernização da infraestrutura de TI da **Farmácia Abstergo (Fictícia)**. O objetivo foi desenhar uma arquitetura na **Amazon Web Services (AWS)** capaz de substituir o data center físico (On-Premises), visando redução de custos operacionais (TCO), alta disponibilidade para o e-commerce e segurança de dados sensíveis de pacientes.

## 🎯 O Desafio (Cenário)

A empresa enfrentava custos elevados de manutenção de hardware, desperdício de energia com servidores ligados 24/7 sem demanda e riscos de *downtime* em períodos de pico (ex: Black Friday), além de preocupações com a integridade de receitas médicas digitais.

## 🏗️ Arquitetura da Solução

A solução foi estruturada em três pilares principais de serviços AWS:

### 1. Computação Elástica (Amazon EC2 + Auto Scaling)
- **Problema:** Servidores ociosos na madrugada e travamentos em picos de acesso.
- **Solução:** Implementação de instâncias EC2 com *Auto Scaling*.
- **Resultado:** A infraestrutura cresce ou diminui automaticamente conforme a demanda, gerando uma economia estimada de **40% a 60%** em computação.

### 2. Banco de Dados Gerenciado (Amazon RDS)
- **Problema:** Rotinas manuais de backup e risco de perda de dados de vendas.
- **Solução:** Migração para Amazon RDS com funcionalidade *Multi-AZ*.
- **Resultado:** Alta disponibilidade (SLA 99,9%), backups automáticos e replicação de dados para prevenção de falhas.

### 3. Armazenamento Seguro (Amazon S3)
- **Problema:** Discos rígidos locais cheios e risco de perda de receitas médicas.
- **Solução:** Armazenamento de arquivos estáticos e documentos no S3.
- **Resultado:** Durabilidade de **99,999999999% (11 noves)**, conformidade com leis de dados (LGPD) e custo reduzido de armazenamento.

## 💰 Benefícios de Negócio

* **CapEx para OpEx:** Eliminação do alto investimento inicial em hardware físico.
* **Redução de TCO:** Projeção de **35% de economia** no Custo Total de Propriedade no primeiro ano.
* **Segurança:** Criptografia de ponta e conformidade com normas de saúde.

## 📂 Estrutura do Repositório

```bash
/
├── docs/              # Relatórios técnicos e executivos
├── diagrams/          # Diagramas de arquitetura e rede
├── costs/             # Planilhas de estimativa de custos (TCO)
└── README.md          # Resumo do projeto


