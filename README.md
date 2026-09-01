# GRUPO 10

## Integrantes do Grupo

- KARLA MARIA RAMOS DA SILVA - RA: 10441405
- LUANA ISABELLA XAVIER PORTO - RA: 10443026 
- GUSTAVO AZEVEDO GOMYDE - RA: 10424543  
- RAFAEL HESSEL SICHETTI - RA: 10375395

## TEMA

Produto Analítico: Previsão e análise de séries temporais de focos de queimadas no Brasil.

## OBJETIVO

O objetivo principal do projeto é desenvolver um produto analítico que contemple a análise e a modelagem da série temporal do número de focos de queimadas no Brasil. Entre as metas específicas, destacam-se:
- Caracterizar a série temporal, identificando seus componentes fundamentais: tendência (direção de crescimento ou decaimento), sazonalidade (padrões regulares ligados às estações seca e chuvosa), ciclos eventuais e a presença de ruído (variações irregulares).
- Definir a técnica de modelagem mais adequada para a base escolhida.
- Construir um modelo preditivo capaz de estimar o volume de focos de calor futuros, fornecendo métricas de suporte à decisão.

## Estrutura do Repositório

| Atributo | Descrição |
|---|---|
| `data_hora_gmt` | Data e hora da detecção do foco, fundamental para a ordenação dos registros no tempo. |
| `lat` e `lon` | Coordenadas geográficas precisas do evento (latitude e longitude). |
| `satelite` | Identificação do sensor de captura de imagem (ex.: satélite GOES-19). |
| `municipio`, `estado`, `bioma` | Dados categóricos e de agrupamento espacial, como os biomas da Amazônia e Cerrado. |
| `precipitacao`, `risco_fogo`, `numero_dias_sem_chuva`, `frp` | Fatores meteorológicos associados e poder relativo do fogo no instante da detecção. |


## Link do Dataset Público

Portal INPE - Estatísticas e Dados Abertos do Programa Queimadas - https://data.inpe.br/queimadas/estatisticas/?tipo=estados
