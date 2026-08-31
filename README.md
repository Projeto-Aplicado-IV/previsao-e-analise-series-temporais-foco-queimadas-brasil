# previsao-e-analise-series-temporais-foco-queimadas-brasil

## Integrantes do Grupo

- ANNA TERESA SOARES SACCHI - RA: 10441273  
- GLEIDER MACKEDANZ DE CAMPOS - RA: 10433464  
- GUSTAVO AZEVEDO GOMYDE - RA: 10424543  
- KELLY HARO VASCONCELLOS - RA: 10441014

## TEMA

Produto Analítico: Previsão e análise de séries temporais de focos de queimadas no Brasil.

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
