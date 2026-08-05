# Layout do CSV

Este documento descreve as colunas que compõem o arquivo .csv utilizado pelo pipeline, bem como detalhes adicionais como obrigatoriedade e exemplos.

### CSV
|Coluna|Tipo|Obrigatorio|Exemplo|
|------|----|-----------|-------|
|codigo_material|Texto|Sim|MAT2141|
|descrição|Texto|Sim|Motor Trifásico 220VCA|
|preço|Decimal|Sim|15.83|
|unidade|Texto|Sim|KG|
|codigo_fornecedor|Texto|Sim|FOR9821|
|categoria|Texto|Sim|Elétrica|

## Especificações do arquivo

- Formato: CSV
- Codificação: UTF-8
- Primeira linha: Cabeçalho
- Separador decimal: `.`
- Delimitador de colunas: `,`