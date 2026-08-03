## Padronização Geral

Todos os campos textuais deverão:

- remover espaços excedentes;
- remover espaços no início e no final;
- padronizar a capitalização;
- utilizar codificação UTF-8.

# Regras de Negócio

Este documento descreve as regras de negócio e os critérios de validação aplicados aos registros do arquivo CSV utilizado como entrada do pipeline.

Cada coluna possui restrições específicas que serão verificadas durante o processamento dos dados. Caso alguma regra seja violada, o registro poderá ser tratado automaticamente ou encaminhado para rejeição, conforme a regra implementada.

| Campo | Obrigatório | Regra de Validação | Exemplo |
|Descrição do Material|Sim|A descrição do material não precisa ser única|Motor Trifásico 220VCA|
|Código do Material|Sim|Código Único com até 10 caracteres|MAT1958|
|Código do Fornecedor|Sim|Deve estar associado a um código de fornecedor existente|FOR4124|
|Categoria|Sim|Deve estar associado a uma categoria existente|Elétrico|
|Status|Sim|Deve ser ativo ou inativo|Ativo|
|Preço|Sim|Deve ser maior que zero|159,90|
|Unidade|Sim|Deve ser UN, M, KG, ou L, sem espaço excedente ao valor|15KG|
|Validade|Condicional|Obrigatório apenas para materiais classificados como perecíveis. Deve conter a data de validade no formato MM/AAAA|06/2028|