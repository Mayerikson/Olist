# Olist


# Desafio Técnico - Programa Trainee triggo.ai 2025

Este repositório contém a solução desenvolvida para o desafio técnico do Programa Trainee triggo.ai de Excelência em Engenharia de Dados e DataOps 2025. O objetivo do projeto é analisar dados históricos de e-commerce da Olist para gerar insights estratégicos e desenvolver soluções com base em Python, SQL e boas práticas de Engenharia de Dados.

## 📁 Dataset

Utilizamos o "Brazilian E-commerce Public Dataset by Olist", disponível no Kaggle:
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

## ✅ Como Executar o Projeto

1. Clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git

2.Instale as dependências:

pip install -r requirements.txt

3.Execute o notebook Olist.ipynb no Jupyter ou Google Colab.


🔍 Principais Análises e Resultados
1. 📦 Preparação dos Dados
Foram tratadas duplicatas e valores nulos em diversas tabelas.

Um modelo relacional foi construído ligando customers, orders, products, sellers, order_items, order_reviews, entre outras.

2. 📊 Análise Exploratória de Dados
Volume de Pedidos por Mês: Identificada leve sazonalidade entre fim de ano e promoções.

Tempo de Entrega: A média gira em torno de 12 dias, com grande dispersão.

Frete x Distância: Correlação positiva, mas com outliers que afetam a linearidade.

Categorias com Maior Faturamento: cama_mesa_banho, relogios_presentes, moveis_decoracao.

Estados com Maior Ticket Médio: DF, MT e ES se destacam.

3. 🧠 Soluções de Problemas de Negócio
Retenção de Clientes: Apenas 3,12% dos clientes compram mais de uma vez — oportunidade para ações de fidelização.

Predição de Atraso:

Definido como pedidos entregues após a data estimada.

Modelo de Random Forest atingiu boas métricas (ex: AUC e recall).

Segmentação de Clientes:

K-Means com 3 clusters baseado em valor total, tempo de entrega e review.

Estratégias personalizadas sugeridas para cada grupo.

Satisfação do Cliente:

Principais fatores: tempo de entrega, estado de destino e tipo de produto.

4. 📈 Dashboards e Visualizações
Gráficos de evolução temporal com filtros de estado e categoria.

Mapa de calor de vendas por estado.

Relação entre avaliação do cliente e tempo de entrega.

Análise de desempenho dos vendedores.

🧪 Tecnologias Utilizadas
Python (Pandas, NumPy, Matplotlib, Seaborn, Plotly)

SQL via SQLite

Scikit-learn

Jupyter Notebook
