# Aula 2 intesivão de python Analise de Dados

usando o pandas para ler podemos usar a função  read_ o tipo de arquivo,
quando usamos o jupyter podemos usar o metodo display() para exibir

### read_... parametros

- encoding= : serve para aceitar alguns tipos de caracteres;
se for usar utf-8 usamos os "latin"
- sep= : serve para dizer para o pandas qual o separador da base de dados;

## Tratamento de dados com python: 

"Informações que não me ajudam, me atrapalham."

deletando uma coluna com python -> usamos o nome da tabelacom o drop()

- drop(): parametros do drop -> nome da coluna, axis

axis = 0 quando for uma linha e 1 quando for coluna
### tratando o tipo de uma coluna
 caso você precise mudar o tipo de uma coluna, podemos usar um metodo do pandas no caso do exemplos usamos o to_numeric();
 parametros do to_numeric(): -> 
    - nome da coluna,
    - errors : podemos usar tres opções o 'coerse', 'ignore', 'raise', o coerse força o valor a se tornar numerico ou transforma ele em NAN;

### dropna():
serve para jogar linhas com valor vazio fora
    - tabela.dropna() 

### info(): 
mostra todas as colunas da tabela

### describe():
serve para descrever a base de dados, porém só colunas numericos, ela tras

## Usando o plotly:

primeiro precisamos installar o plotly com o comando, pip install plotly;

depois iremos escolher o tipo de graficos que vamos utilizar para o exemplo histogram
import plotly.express as px
grafico = px.histogram(tabela, x='coluna pra eixo x', y='coluna para o eixo y')

depois para exibir podemos usar:

grafico.show()

### histfunc= : 
nesse parametro do gráfico podemos mudar a função que esta sendo usada, por padrão é sum(); string

### text_auto= :
parametro para dizer se as colunas vao ter texto, padrão false; boolean

### nbins= : 
parametro para aumentar ou diminuir a quantidade de faixas no grafico; vlr numerico



# A analise de fato: 



