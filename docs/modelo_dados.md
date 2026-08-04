# Modelo de Dados

Este documento descreve as tabelas que compõem o modelo relacional utilizado pelo pipeline, bem como seus principais atributos, chaves e relacionamentos.

### Material
|Campo|Tipo|Observação|
|-----|----|----------|
|Código|VARCHAR(10)|Primary Key (PK)|
|Descrição|VARCHAR(100)|Sem observação|
|Preço|numeric|Sem observação|
|Unidade|VARCHAR(2)|Sem observação|
|Status|boolean|Ativo ou Inativo|
|Código_Fornecedor|VARCHAR(10)|Foreign Key (FK - Código - Tabela Fornecedor)
|ID_Categoria|INTEGER|(FK - ID - Tabela Categoria)|

### Fornecedor
|Campo|Tipo|Observação|
|-----|----|----------|
|Código|VARCHAR(10)|Primary Key (PK)|
|Nome|VARCHAR(100)|Sem observação|
|Status|boolean|Ativo ou Inativo|

### Categoria
|Campo|Tipo|Observação|
|-----|----|----------|
|ID|serial|Primary Key (PK)|
|Nome|VARCHAR(100)|Sem observação|
|NCM|VARCHAR(8)|Sem observação|
|Status|boolean|Ativo ou Inativo|

### Fornecedor_Categoria
|Campo|Tipo|Observação|
|-----|----|----------|
|ID|serial|Primary Key (PK)|
|Código_Fornecedor|VARCHAR(10)|(FK - Código - Tabela Fornecedor)|
|ID_Categoria|INTEGER|(FK - ID - Tabela Categoria)|


## Links dos diagramas completos
Mais detalhes podem ser encontradas nos sites a seguir:

Diagrama ER: 'link do miro'
Tabelas relacionais: 'link do miro'
