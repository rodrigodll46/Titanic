# Titanic


## Introdução

O naufrágio do RMS Titanic, em 1912, é um dos desastres mais conhecidos da história. Durante sua viagem inaugural, o navio colidiu com um iceberg no Oceano Atlântico Norte e acabou afundando, resultando na morte de centenas de passageiros e tripulantes.

## Objetivo

Este projeto tem como objetivo identificar e analisar os principais fatores que influenciaram a sobrevivência dos passageiros do Titanic. Para isso, foi realizada uma Análise Exploratória de Dados (EDA) utilizando um dataset público. A proposta é compreender melhor o perfil dos passageiros e investigar quais características impactaram suas chances de sobrevivência.

## Importação e Carregamento dos Dados

Foram utilizadas as seguintes bibliotecas:

* **Pandas**: manipulação de dados
* **NumPy**: cálculos numéricos
* **Matplotlib** e **Seaborn**: visualização de dados

O conjunto de dados foi obtido via GitHub e carregado diretamente no notebook.

## Entendimento Inicial dos Dados

O dataset possui:

* 891 registros (passageiros)
* 12 colunas com informações como idade, sexo, classe, tarifa e sobrevivência

Após uma análise inicial (`info()` e `describe()`), foram selecionadas as variáveis mais relevantes para o estudo:

* Survived
* Pclass
* Sex
* Age
* SibSp
* Parch
* Fare
* Embarked

## Limpeza e Tratamento dos Dados

As etapas de limpeza incluíram:

* Remoção de registros duplicados
* Tratamento de valores nulos:

  * **Idade (Age)** preenchida com a mediana
  * **Embarque (Embarked)** preenchido com a moda
* Ajuste dos tipos de dados para categorias

## Análise Exploratória de Dados (EDA)

### Sobrevivência Geral

A maioria dos passageiros não sobreviveu ao naufrágio.

### Sobrevivência por Gênero

Mulheres tiveram uma taxa de sobrevivência significativamente maior que homens, indicando prioridade no resgate.

### Sobrevivência por Classe

* Passageiros da **1ª classe** tiveram maior taxa de sobrevivência
* Passageiros da **3ª classe** tiveram as menores chances

Isso sugere influência de fatores socioeconômicos e acesso aos botes salva-vidas.

### Sobrevivência por Idade

Crianças apresentaram maior taxa de sobrevivência, reforçando a hipótese de prioridade durante o resgate.

### Análises Combinadas

* **Gênero + Classe**: mulheres tiveram maior sobrevivência em todas as classes
* **Idade + Gênero**: crianças e mulheres foram os grupos mais favorecidos

## Principais Insights

* Gênero foi o fator mais relevante
* Passageiros da 1ª classe tiveram vantagem significativa
* Crianças apresentaram maior taxa de sobrevivência
* Homens da 3ª classe foram os mais afetados

## Conclusão

A análise mostrou que os principais fatores que influenciaram a sobrevivência no Titanic foram **gênero, classe social e idade**. Mulheres e passageiros da primeira classe tiveram maiores chances de sobreviver, enquanto homens da terceira classe enfrentaram as menores.

Este projeto demonstra como a análise de dados pode ajudar a entender eventos históricos e revelar padrões importantes, contribuindo para interpretações mais profundas e tomadas de decisão baseadas em dados.

---

*Projeto desenvolvido para fins de estudo em análise de dados por Rodrigo Correa Dallastra da Silva.*
