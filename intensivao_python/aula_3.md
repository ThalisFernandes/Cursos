### web scraping com selenium

# passo a passo

## passo 1  :entrar na interet (abrir o navegador)
instalar o selenium: 
pip install selenium

baixar o webdriver do navegador que vc usa: firefox ou chrome


importar o selenium

acessar o site com o selenium

## passo 2 : importar a base de dados

primeiro usaremos o pandas para importar a base de dados 

ler a tabela com o pandas



## passo 3 : para cada produto  

## passo 4 : pegar o preço atual do produto
com selenium usando o xpath

selenium.findelement('xpath', 'xpath do elemento').get_attribute('') "nesse caso sera o value"

## passo 5 : Atualizar o preço na base de dados

com o pandas podemos usa o comando:

tabela.loc[linha, nome_da_coluna] = vlr para alterar


## passo 6 : Decidir quais produtos a gente vai comprar
o proprio pandas pode fazer isso com a seleção de coluna com a seguinte sintaxe

tabela['comprar'] = tabela['preço_atual'] < tabela['preço_ideal']

assim será retorna true quanto o valor do preço atual for menor que o preço ideal, podemos também usar os operadores lógicos de <=, >, >=, ==, !=, 

## passo 7 : Exportar a base de dados atualizada



