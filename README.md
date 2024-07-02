## Introdução

Este repositório contém dados analíticos sobre hubs de distribuição e pontos de entrega da Loggi em Brasília, visando melhorias na logística de transporte da empresa.

## Pacotes e Bibliotecas Utilizados

- geopandas
- json
- pandas
- geopy
- matplotlib
- seaborn

## Carregamento e Exploração de Dados

Os dados foram extraídos de um arquivo JSON e carregados em um DataFrame pandas para análise.

## Manipulação de Dados

### Normalização de Dados Aninhados

A coluna 'origin' dos dados continha informações aninhadas em JSON, que foram normalizadas utilizando o método `pd.json_normalize`.

### Explodindo Dados em Listas

Utilizou-se o método `explode` para transformar cada elemento de uma lista em uma linha separada no DataFrame.

### Enriquecimento de Dados

Realizou-se a geocodificação reversa das coordenadas dos hubs para obter informações detalhadas de localização, como cidade e bairro.

### Normalização e Seleção de Dados

As informações geocodificadas foram normalizadas e selecionadas para extrair apenas as colunas relevantes (cidade e bairro).

## Resultados

Os dados enriquecidos foram combinados com o DataFrame original, proporcionando uma visão detalhada das localizações dos hubs e pontos de entrega em Brasília.

## Conclusão

Este projeto demonstra a aplicação de técnicas de manipulação e enriquecimento de dados geográficos para melhorar a eficiência logística da Loggi em Brasília.
