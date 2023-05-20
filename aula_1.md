# aula 1 - intesivão de python;

## Passos iniciais:

- instalar o jupiter notebook;
- instalar o pyautogui;
- escrever o passo a passo do processo;

### para instalar bibliotecas com o Jupiter
usamos "!" antes do comando do pip na celula do jupiter
EX: !pip install pyautogui

### sobre o pyautogui

precisamos conheçer alguns dos principais comandos do pyautogui que são os seguintes:
pyautogui.click -> clica com o mouse
pyautogui.write -> escreve um texto
pyautogui.press -> aperta uma unica tecla
pyautogui.hotkey -> aperta uma combinação de teclas

sintaxe do hotkey
pyautogui.hotkey("ctrl", "t")

## Pausa do proprio pyautogui

é uma pausa interna da propria biblioteca a sintaxe é a seguinte:
pyautogui.PAUSE = 

uma pausa entre cada comando do pyautogui, ela serve para os comandos do proprio pyautogui n atropelarem uns aos outros.

## pyautogui.click parametros

clicks = quantidade de cliques que vc vai dar
button = butão do mouse que você vai apertar

## Usando o pandas
pandas ele ja vem instalado no jupiter, ele serve para trabalhar com base de dados;
caso não esteja usando o jupiter será preciso installar os seguintes pacotes: 
- pip install pandas
- pip install openpyxl
- pip install numpy

"sempre que for passar um caminho de um arquivo para o python, sempre usar o 'r' antes da string"

para ler uma base de dados com o panda, o pandas tem o read_... podendo ser csv, html ...
### pandas.read_... parametros
 - sep = é o separador da planilha para poder ajudar a separar os elementos, para eles não ficar todos em uma coluna;

### fazendo operações com o pandas 

para selecionar uma coluna de uma tabela no pandas usamos [];

soma -> .sum()
media -> .mean()


## passo a passo do processo;



## automação de sistemas e processos com python;

