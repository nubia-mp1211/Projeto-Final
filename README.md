# Projeto-Final
Este projeto consiste em determinar o número de brasileiros vacinados contra COVID-19, usando o Modelo Prophet para previsão de Séries Temporais em Python.

O banco de dados foi coletado no site do Governo Federal (gov.br) e através de API, foi possível acessar as informações criando um arquivo contendo dados necessários para fazer a previsão. Os dados obtidos estão de acordo com a Lei Geral de Proteção de Dados (LGPD) e a pessoa vacinada é identificada apenas com um número gerado randomicamnete (ID) para saber se tomou a primeira dose, segunda dose ou dose ünica.

Como a base de Vacina contém muitos dados, foi gerando uma amostragem desse arquivo, definindo uma porcentagem da banco de dados para facilitar a execução dos códigos. 

A sequencia de execução dos programas:
1) Rodar-PRINCIPAL-com-ALGUNS-Campos-Vacina, que faz a coleta da base de dados no site do Governo Federal, gerando arquivo Vacina-AA-MM-DD-HH:MM (dia 26/5/2021 o arquivo Vacina - tamanho de 20GB)
2) Gerando-Amostra_Alguns-Campos, este programa gera o arquivo  BD-AMOSTRA-Alguns-26-05-21 que contém uma porcentagem do base de dados Vacina, onde utilizo o percentual de 0.001, isto é, para 1.000 vacinados faço a seleção randomicamente desse arquivo BD-AMOSTRA-Alguns-26-05-214). 
3) Está disponível a base de dados AMOSTRA para futuro testes. 
4) Alguns programas que contém informações que foram trabalhadas para obter os gráficos:
5) Grafico-Fabricantes-vacinas = mostra os fabricantes das vacinas disponíveis no Brasil e gráfico acumulado
6) Primeira-Segunda-Doses = apresenta o total de vacinados no Brasil com a primeira e segunda dose 
7) Faço uma análise dos brasileiros vacinados no Estado de São Paulo (SP) e nas 5 regiões do Brasil: NORTE, NORDESTE, CENTRO-OESTE, SUDESTE e SUL do Brasil.
8) E finalmente, ATUAL-Tratando-Vacinados e Previsoes = este programa faz toda análise e utiliza o Modelo Machine Learning, Prophet para fazer a previsão de quando teremos toda população brasileira vacinada.
