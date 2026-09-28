# qualidade-ar-capitais
Projeto de Ciência de Dados para análise e previsão da qualidade do ar nas capitais brasileiras utilizando séries temporais e Machine Learning.
Título

Análise e Previsão da Qualidade do Ar nas Capitais Brasileiras

Autora

Ingryd Cristine Hidalgo Sella
RA: 10424934

Sobre o projeto

Explique o problema que vocês estão tentando resolver.

Objetivos

Por exemplo:

analisar a qualidade do ar;
identificar padrões temporais;
estudar a relação com variáveis meteorológicas;
desenvolver modelos de previsão;
comparar modelos estatísticos e Machine Learning;
disponibilizar os resultados publicamente.

Tecnologias
Python
Pandas
NumPy
Matplotlib
Scikit-learn
Statsmodels
XGBoost
Jupyter Notebook

## Fontes dos dados

O projeto utilizará prioritariamente dados provenientes de fontes oficiais
e primárias, evitando bases secundárias ou previamente processadas.

### Qualidade do ar

Os dados de qualidade do ar serão obtidos por meio do **MonitorAr**, sistema
do Ministério do Meio Ambiente e Mudança do Clima (MMA), que reúne informações
provenientes de estações oficiais de monitoramento da qualidade do ar
integradas ao sistema.

Os dados disponibilizados incluem registros das estações de monitoramento
e informações relacionadas aos poluentes atmosféricos. O Portal de Dados
Abertos do MMA disponibiliza os conjuntos de dados do MonitorAr em arquivos
CSV, incluindo dados referentes aos anos de 2022, 2023, 2024 e 2025.

Fonte:
https://dados.mma.gov.br/dataset/ar-puro-monitorar

### Dados meteorológicos

As variáveis meteorológicas serão obtidas prioritariamente por meio do
**Instituto Nacional de Meteorologia (INMET)**, utilizando o Banco de Dados
Meteorológicos (BDMEP).

O BDMEP disponibiliza séries históricas de dados meteorológicos provenientes
da rede de estações do INMET. Essas informações poderão ser utilizadas para
relacionar as condições meteorológicas com o comportamento dos poluentes
atmosféricos.

Fonte:
https://bdmep.inmet.gov.br/

### Dados complementares

Quando necessário, poderão ser utilizados dados complementares de órgãos
ambientais oficiais, desde que a origem, metodologia de coleta e condições
de utilização dos dados sejam devidamente documentadas no projeto.

Como referência complementar para dados de qualidade do ar no Estado de São
Paulo, poderá ser consultada a rede automática da CETESB, que disponibiliza
informações horárias e boletins de qualidade do ar de suas estações.

Fonte:
https://sistemasinter.cetesb.sp.gov.br/Ar/

## Metodologia

O projeto será desenvolvido utilizando uma abordagem de Ciência de Dados
aplicada à análise e previsão de séries temporais.

O processo será dividido nas seguintes etapas:

### 1. Coleta

Serão coletados dados históricos de qualidade do ar e dados meteorológicos
provenientes de fontes oficiais. Os registros serão organizados de acordo
com sua localização e referência temporal.

↓

### 2. Tratamento

Será realizada a limpeza dos dados, incluindo identificação de valores
ausentes, duplicidades, inconsistências, formatos inadequados de data e hora
e possíveis valores extremos.

↓

### 3. Integração

Os dados de qualidade do ar serão relacionados aos dados meteorológicos
considerando a localização das estações e a correspondência temporal entre
as observações.

↓

### 4. Análise exploratória

Serão analisadas as características das séries temporais, buscando identificar
tendências, sazonalidade, padrões horários, diários e mensais, além da
relação entre os poluentes e as condições meteorológicas.

↓

### 5. Engenharia de atributos

Serão criadas variáveis derivadas dos dados históricos, como valores
defasados, médias móveis, máximos e mínimos de períodos anteriores, além de
variáveis temporais como hora, dia da semana, mês e estação do ano.

↓

### 6. Modelagem

Serão avaliadas diferentes abordagens para previsão de séries temporais,
incluindo modelos estatísticos, como ARIMA/SARIMA, e algoritmos de Machine
Learning, como Random Forest e/ou XGBoost.

↓

### 7. Previsão

Os modelos treinados serão utilizados para realizar previsões dos níveis
dos poluentes em períodos futuros, preservando a ordem cronológica dos dados.

↓

### 8. Avaliação

Os resultados serão avaliados utilizando métricas como MAE (Mean Absolute
Error) e RMSE (Root Mean Squared Error). Também serão comparados os valores
observados e previstos por meio de visualizações.

↓

### 9. Dashboard

Os resultados serão disponibilizados por meio de um dashboard analítico,
apresentando informações históricas, indicadores, gráficos e previsões de
forma acessível ao usuário.

## ODS

O projeto está relacionado principalmente à **ODS 11 – Cidades e Comunidades
Sustentáveis**, da Organização das Nações Unidas (ONU).

A relação ocorre especificamente com a **Meta 11.6**, que estabelece a
necessidade de reduzir o impacto ambiental negativo das cidades, com atenção
especial à qualidade do ar.

O projeto contribui para esse objetivo ao transformar dados oficiais de
qualidade do ar e condições meteorológicas em informações analíticas,
previsões e visualizações que podem ser disponibilizadas publicamente.

Fonte:
https://brasil.un.org/pt-br/sdgs/11
