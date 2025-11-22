
# 📊 Análise de Desempenho e Estratégia de Varejo

Este projeto consiste em uma análise exploratória de dados (EDA) focada na tomada de decisão estratégica para uma rede de varejo composta por quatro filiais. O objetivo principal foi identificar padrões de consumo, eficiência operacional e saúde financeira para recomendar qual unidade deveria ser descontinuada (vendida).

## 🎯 Objetivo do Projeto

O Senhor João, proprietário da rede, precisa reestruturar o negócio e decidiu vender uma das suas quatro lojas. A análise visa responder à pergunta: **"Qual loja deve ser vendida?"** baseando-se em dados concretos e não apenas em intuição.

Os principais KPIs analisados foram:

-   Faturamento total por loja.
    
-   Mix de produtos vendidos e categorias mais populares.
    
-   Satisfação do cliente (Média de avaliações).
    
-   Eficiência logística (Custo médio de frete).
    
-   Distribuição geográfica das vendas.
    

## 🛠️ Tecnologias Utilizadas

O projeto foi desenvolvido utilizando a linguagem **Python** e as seguintes bibliotecas para manipulação e visualização de dados:

-   [**Pandas**](https://pandas.pydata.org/ "null")**:** Para carregar, limpar, transformar e agregar os dados das tabelas CSV.
    
-   [**Matplotlib**](https://matplotlib.org/ "null")**:** Para a criação de gráficos básicos (linhas, dispersão).
    
-   [**Seaborn**](https://seaborn.pydata.org/ "null")**:** Para visualizações estatísticas avançadas e esteticamente agradáveis (gráficos de barras, heatmaps).
    

## 📂 Estrutura dos Dados

O dataset é composto por 4 arquivos CSV (`loja_1.csv`, `loja_2.csv`, `loja_3.csv`, `loja_4.csv`), onde cada arquivo representa as transações de uma filial. As colunas principais são:

Coluna

Descrição

`Produto`

Nome do item vendido.

`Categoria do Produto`

Classificação (ex: móveis, eletrônicos).

`Preço`

Valor da venda (Faturamento).

`Frete`

Custo de envio pago pelo cliente.

`Data da Compra`

Data da transação.

`Vendedor`

Nome do vendedor responsável.

`Local da compra`

Estado (UF) do cliente.

`Avaliação da compra`

Nota dada pelo cliente (1 a 5).

`lat` / `lon`

Coordenadas geográficas do destino da entrega.

## 🚀 Como Executar o Projeto

### Pré-requisitos

Certifique-se de ter o Python instalado. Recomenda-se o uso de um ambiente virtual (venv) ou o Google Colab/Jupyter Notebook.

### Instalação

Clone este repositório (ou baixe os arquivos) e instale as dependências listadas:

```
pip install pandas matplotlib seaborn

```

### Execução

1.  Certifique-se de que os arquivos `loja_1.csv` até `loja_4.csv` estão no mesmo diretório do script.
    
2.  Execute o notebook ou script Python principal para gerar os gráficos e o relatório.
    

```
# Exemplo de carregamento inicial no script
import pandas as pd

df1 = pd.read_csv('loja_1.csv')
# ... (código de análise)

```

## 📊 Principais Descobertas

Durante a análise, identificamos os seguintes pontos chaves:

1.  **Liderança Financeira:** A **Loja 1** possui o maior faturamento acumulado, sendo o pilar financeiro da rede, apesar de ter custos de frete mais altos.
    
2.  **Satisfação do Cliente:** As lojas possuem desempenho similar, mas a **Loja 3** se destaca levemente com a melhor média de avaliações (4.05).
    
3.  **Desempenho Geográfico:** Todas as lojas competem pelos mesmos mercados (Sudeste e Sul), não havendo exclusividade regional que justifique manter uma loja específica apenas por sua localização.
    

### ✅ Conclusão Final

A recomendação estratégica é a **venda da Loja 4**.

-   **Motivo:** Apresentou o menor faturamento total entre todas as unidades. Embora seja eficiente logisticamente, ela não gera volume de vendas suficiente para superar as outras filiais, e sua ausência causa o menor impacto financeiro no grupo.
    

## ✒️ Autor

Desenvolvido por Marcelo Santos como parte de um desafio de Ciência de Dados.

_Este projeto é fictício e foi criado para fins educacionais de análise de dados._
