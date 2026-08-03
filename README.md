# Pipeline de Qualidade de Dados para Cadastro de Materiais

## Sobre o projeto

Este projeto simula um pipeline corporativo de qualidade de dados para cadastro de materiais, inspirado em processos utilizados por empresas que trabalham com sistemas ERP, como o SAP.

O objetivo é reproduzir o fluxo de validação, tratamento e integração de dados mestres (Master Data), utilizando um arquivo CSV contendo inconsistências propositalmente inseridas para simular problemas encontrados no ambiente corporativo.

O projeto foi desenvolvido com foco em aprendizado prático de Engenharia de Dados, Análise de Dados e Governança de Dados, utilizando tecnologias amplamente empregadas no mercado.

---

## Problema de negócio

Em muitas empresas, novas solicitações de cadastro de materiais são enviadas por diferentes áreas por meio de planilhas ou arquivos CSV.

Como esses arquivos geralmente são preenchidos manualmente, é comum encontrar problemas como:

- códigos duplicados;
- descrições incompletas;
- campos obrigatórios não preenchidos;
- unidades de medida inválidas;
- preços negativos;
- fornecedores inexistentes;
- registros duplicados;
- diferenças de padronização de texto;
- caracteres especiais;
- tipos de dados incorretos.

Caso essas inconsistências não sejam identificadas antes da integração com o ERP, elas podem comprometer a qualidade do cadastro, gerar retrabalho e impactar processos como compras, planejamento, produção e controle de estoque.

---

## Solução

Este projeto implementa um pipeline de qualidade de dados capaz de:

- realizar a leitura de arquivos CSV;
- executar análises de Data Profiling;
- validar regras de qualidade dos dados;
- tratar inconsistências quando possível;
- registrar logs de processamento;
- separar registros aprovados e rejeitados;
- carregar os dados aprovados em um banco de dados;
- disponibilizar indicadores em um dashboard desenvolvido no Power BI.

---

## Tecnologias

- Python
- Pandas
- PostgreSQL
- SQL
- Power BI
- Git
- GitHub

---

## Fluxo do projeto

```text
CSV
        ↓
Extração
        ↓
Data Profiling
        ↓
Validação
        ↓
Tratamento
        ↓
Logs
        ↓
Banco de Dados
        ↓
Dashboard Power BI
```

---

## Objetivo

O principal objetivo deste projeto é construir um pipeline de dados semelhante ao utilizado em ambientes corporativos, aplicando conceitos de Engenharia de Dados, Qualidade de Dados, ETL e Governança de Dados em um cenário inspirado em processos de Master Data Management (MDM).