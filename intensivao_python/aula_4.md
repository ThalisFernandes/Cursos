# Aula 4 - Projeto ciência de dados - Previsão de preços

Objetivo > Prever o preço de barco que vamos vender baseado nas caracteristicas do barco como ano, tamanho, tipo de barco, se e novo ou usado, qual material usado, etc.


### Importando a base de dados: 

usaremos o pandas 

### Ajuste dos dados 

### Análise Exploratória :
-> Meu palpite: Tipo do barco / Tipo de venda

como cálcular a correlação da tabela:

tabela.corr() -> serve para cálcular correlação entre colunas;

sintaxe :: 

tabela.corr()["nomeColuna"] -> tabela.corr()[["nomeColuna"]] 

oque é correlação: 
Correlação é um número de 0 a 1 que serve para indicar quando duas informações estão cerrelacionadas uma a outra;

vamos usar o seaborn e matplotlib, para os novos graficos: 

import seaborn as sns
import matplotlib.pyplot as plt




# Modelagem + algoritmos :

## Preparação para a IA: 

### Passo

### Criação e treino da IA: 
- separara a base em valores de X e Y ;
    sabendo que Y será quem a minha IA deve prever e X oque ela vai usar como info para prever o Y;

y = tabela['coluna_para_a_ia_prever']

x = tabela.drop('coluna_para_a_ia_prever', axis=1)

sklearn -> pacote para treinar inteligencias artificiais com varios modelos de inteligencias artificiais para treinar;

from sklearn.model_selection import  train_test_split

x_treino, x_text, y_treino, y_teste = train_test_Split(x, y, test_size=0.3, random_state=1)

@params :

random_state  : ele serve para evitar que cada vez que o código seja rodado não faça o embaralhamento da base;

test_size    :  serve para dizer o tamanho da base de teste e treino


#### Importanddo a Inteligencia Artificial: 
from sklearn.linear_model import LinearRegression
from sklearn.ensemble import RandomForestRegressor


#### Criando a Inteligência Artificial
definimss uma variavel para receber o modelos de inteligencia assim: 

arvore = RandomForestRegressor()
regressao = LinearRegression()



#### Treinando a IA: 

passaremos os dados que foram separados para que a IA possa aprender usando o metodo fit(), 
arvore.fit(x_treino, y_treino)
regressao.fit(x_treino, y_treino)


#### Previssões com a IA: 

para isso precisaremos usar o metodo predict() da 

### Interpretação de Resultados :

nessa parte podemos usar o seaborn para fazer a exibição dos dados obtidos pela IA

