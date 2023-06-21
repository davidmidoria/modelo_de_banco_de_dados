# modelo_de_banco_de_dados

Foi solicitado a criação de um banco de dados com o objetivo de analisar as tecnologias utilizadas pelas empresas e seus colaboradores. Para isso, optou-se por criar um modelo relacional com a intenção de obter insights a partir dos dados coletados.

Antes de criar um banco de dados, é fundamental desenvolver um modelo de banco de dados. O primeiro passo foi a criação do modelo conceitual.

## modelo conceitual. 

O modelo conceitual é essencial para a estruturação do banco de dados, pois considera os relacionamentos entre as entidades e a cardinalidade desses relacionamentos. Ele proporcionará uma visão clara e organizada do domínio em estudo, permitindo identificar as principais entidades envolvidas e suas interações. Esse modelo servirá como base para o desenvolvimento do modelo relacional, que possibilitará a obtenção de insights valiosos a partir dos dados coletados.


![imagem do mmodelo conceitual ](imagens_do_banco/modelo_conceitual.png)



## modelo lógico

Após a criação do modelo conceitual, o próximo passo foi aprimorar o modelo e transformá-lo em um diagrama no modelo lógico. Nesse estágio, foram adicionados atributos, chaves primárias, chaves estrangeiras e relacionamentos que ajudaram a estruturar o banco de dados.

O modelo lógico refina o modelo conceitual e o traduz em termos mais específicos, adequados para a implementação do banco de dados. Ele define as tabelas, os campos de cada tabela, os tipos de dados e as restrições associadas aos dados.

Durante a criação do modelo lógico, foram identificadas as chaves primárias de cada tabela, que são os atributos únicos que identificam de forma exclusiva cada registro. Além disso, as chaves estrangeiras foram utilizadas para estabelecer relacionamentos entre as tabelas, permitindo a consulta e manipulação de dados relacionados.

Com essas melhorias, o modelo lógico está estruturado e pronto para a implementação do banco de dados, fornecendo a base necessária para armazenar e analisar as informações sobre as tecnologias utilizadas pelas empresas e seus colaboradores.

![imagem do ](imagens_do_banco/modelo_logico.png)

## Requisitos

para a criação do banco de dados era necessario responder quatro requisitos 

1. listar as entidades necessarias

2. listar os campos e seus tipo

3. demonstrar o relacionamento entre as tabelas

4. Simular 2 registros para cada entidade


### 1 entidades necessarias

foram necessarias as seguintes entidades

* empresa

* tecnologia

* colaborador

* registro

### 2 principais campos e seus respectivos tipos

os valores serão listados no formato de uma tabela contendo as entdades,  campos e tipos

| *entidade* | *campo* | *tipo* |
|:--------:|:-----:|:----:|
| empresa  | cnpj  | varchar |
| tecnologia | id | integer |
| colaborador | matricula | integer |
| registro | id | integer|

### 3 Como essas entidades estão relacionadas

* empresa esta vinculada a colaborador pelo cnpj

* colaborador esta vinculado a registro pela matricula

* tecnologia esta vinculada a registro pelo id

### 4 simulação  de registros nas entidades

#### empresa

| *cnpj* | *nome* | *segmento*|
|:----:|:----:|:-------:|
| 21.786.344/0001-33. | orange | varejo |
| 32.465.341/0002-23.| redblock | construção|

#### colaborador

| *matricula*| *nome* | *cargo* | *cnpj_empresa*|
|:----:|:----:|:-------:|
| 001 | rogerio | analista | 21.786.344/0001-33|
| 002 | marcio | frontend | 32.465.341/0002-23.|

#### tecnologia

| *id* | *nome* | *area* |
|:----:|:----:|:-------:|
| 1  | vscode | dados |
| 2 | photoshop | marketing|

#### registros

| *id* | *matricula_colaborador* | *id_tecnologia* | *data* |
|:----:|:----:|:-------:|
| 1 | 001 | 1 | 20/06/2023 |
| 2 | 002 | 2 | 15/07/2023 |

