# GRUPO 10

## Integrantes do Grupo

- KARLA MARIA RAMOS DA SILVA - RA: 10441405
- LUANA ISABELLA XAVIER PORTO - RA: 10443026 
- GUSTAVO AZEVEDO GOMYDE - RA: 10424543  
- RAFAEL HESSEL SICHETTI - RA: 10375395

## TEMA

Produto Analítico: Previsão e análise de séries temporais de focos de queimadas no Brasil.

## Introdução

As séries temporais estão presentes em diversas áreas da ciência, sendo fundamentais para a climatologia, finanças e gestão pública. No contexto ambiental, o monitoramento sistemático de variáveis naturais permite a criação de um modelo descritivo e preditivo útil para a sociedade. O presente projeto foca na área de conhecimento de Ciências de Dados aplicada ao Meio Ambiente e Climatologia, dedicando-se à análise da série temporal de focos de queimadas no território brasileiro.
O problema selecionado consiste na dificuldade de antecipar e compreender a distribuição temporal dos focos de incêndio florestal ao longo dos meses e anos. A análise de séries temporais é a investigação de variáveis observadas ao longo do tempo, com a pretensão de realizar previsões para períodos futuros, além de investigar o mecanismo gerador dos dados e descrever apenas o comportamento da série, identificando a existência de tendências, ciclos e variações sazonais.

## Motivações e Justificativa

O Brasil possui biomas de imensa importância global, como a Amazônia e o Cerrado, que sofrem anualmente com a incidência de queimadas. Compreender a dinâmica temporal desses eventos é uma questão de grande relevância ambiental, econômica e de saúde pública, dado que as queimadas afetam a qualidade do ar, destroem a biodiversidade e contribuem para a emissão de gases de efeito estufa.
O estudo analítico dessas séries se justifica pelo potencial de aplicabilidade da solução: ao modelar o comportamento histórico e prever cenários futuros (sejam de curto, médio ou longo prazo), os resultados obtidos poderão servir de apoio para ações governamentais e privadas, como o planejamento logístico de brigadas de incêndio, o controle da degradação ambiental e a alocação eficiente de recursos para contenção em épocas de estiagem severa. As motivações englobam a oportunidade de utilizar modelos estatísticos para extrair valor de bases públicas reais em favor da sociedade civil.


## OBJETIVO

O objetivo principal do projeto é desenvolver um produto analítico que contemple a análise e a modelagem da série temporal do número de focos de queimadas no Brasil. Entre as metas específicas, destacam-se:
- Caracterizar a série temporal, identificando seus componentes fundamentais: tendência (direção de crescimento ou decaimento), sazonalidade (padrões regulares ligados às estações seca e chuvosa), ciclos eventuais e a presença de ruído (variações irregulares).
- Definir a técnica de modelagem mais adequada para a base escolhida.
- Construir um modelo preditivo capaz de estimar o volume de focos de calor futuros, fornecendo métricas de suporte à decisão.

## Descrição da Base de Dados

A base de dados selecionada provém do banco de dados abertos do Instituto Nacional de Pesquisas Espaciais (INPE), através do Programa Queimadas. Trata-se de um conjunto de dados reais e públicos, amplamente utilizado como referência analítica.
Informações disponíveis e Estrutura: A amostragem original consiste em dados diários com granularidade a nível de foco de calor individual. A análise do conjunto de dados bruto demonstra a presença de diversas variáveis estruturadas da seguinte forma:

| Atributo | Descrição |
|---|---|
| `data_hora_gmt` | Data e hora da detecção do foco, fundamental para a ordenação dos registros no tempo. |
| `lat` e `lon` | Coordenadas geográficas precisas do evento (latitude e longitude). |
| `satelite` | Identificação do sensor de captura de imagem (ex.: satélite GOES-19). |
| `municipio`, `estado`, `bioma` | Dados categóricos e de agrupamento espacial, como os biomas da Amazônia e Cerrado. |
| `precipitacao`, `risco_fogo`, `numero_dias_sem_chuva`, `frp` | Fatores meteorológicos associados e poder relativo do fogo no instante da detecção. |

Forma e Período de Coleta: Os dados são coletados de maneira contínua e regular através de sensoriamento remoto via satélite. Para fins da construção da série temporal univariável neste projeto, esses registros pontuais e irregulares serão agrupados temporalmente (através da soma diária, semanal ou mensal do volume de focos), originando uma sequência ordenada de observações igualmente espaçadas ao longo do tempo.
Fonte dos Dados: Portal INPE - Estatísticas e Dados Abertos do Programa Queimadas.

## Link do Dataset Público

Portal INPE - Estatísticas e Dados Abertos do Programa Queimadas - https://data.inpe.br/queimadas/estatisticas/?tipo=estados

## Referências 

DOANE, D. P.; SEWARD, L. E. Estatística aplicada à administração e economia. 4. ed. Porto Alegre: AMGH, 2014.
INSTITUTO NACIONAL DE PESQUISAS ESPACIAIS (INPE). Programa Queimadas: Banco de Dados de Focos. Dados abertos governamentais. Acesso em: 31 ago. 2026.
MORETTIN, P. A.; TOLOI, C. M. C. Análise de séries temporais. 3. ed. São Paulo: Blucher, 2018.
