# Projeto de análise de dados de veículos

## Descrição:
Este projeto tem como objetivo analisar os dados coletados nos últimos anos a partir de centenas de propagandas gratuitas de veículos publicadas diariamente em um site. O objetivo é determinar quais fatores influenciam o preço de um veículo.

## Dados:
O arquivo de dados está localizado em /datasets/vehicles_us.csv

## Pré-processamento de dados:

- Identificação e estudo de valores ausentes
- Conversão de dados para os tipos necessários
- Cálculo e adição de novas colunas (dia da semana, mês, ano, idade do veículo, média de quilometragem por ano)
- Substituição de valores de string por uma escala numérica na coluna condition

## Análise exploratória de dados:

- Estudo dos parâmetros: preço, idade do veículo, quilometragem, número de cilindros e condição
- Construção de histogramas para cada um desses parâmetros
- Determinação dos limites superiores de valores atípicos e remoção desses valores para continuar o trabalho com os dados filtrados
- Construção de novos histogramas com os dados filtrados e comparação com os histogramas anteriores
- Estudo do tempo de vida útil comum de uma propaganda
- Análise do número de propagandas e preço médio para cada tipo de veículo, construção de gráfico para mostrar a dependência do número de propagandas em relação ao tipo de veículo
- Determinação dos fatores que mais influenciam o preço, incluindo análise da relação entre preço e idade, quilometragem, condição, tipo de transmissão e cor dos veículos. Construção de gráficos de extremos, quartis e dispersão para cada variável categórica. Note que as categorias precisam ter pelo menos 50 propagandas para análise.

## Descrição dos dados
O conjunto de dados contém os seguintes campos:
* `price`: preço
* `model_year`: ano do modelo
* `model`: modelo
* `condition`: condição
* `cylinders`: cilindros
* `fuel`: gasolina, diesel etc.
* `odometer`: a quilometragem do veículo quando a propaganda foi publicada
* `transmission`: transmissão
* `paint_color`: cor da tinta
* `is_4wd`: se o veículo é 4 por 4 (tipo Booleano)
* `date_posted`: a data que a propaganda foi publicada
* `days_listed`: dias desde a publicação até a retirada
