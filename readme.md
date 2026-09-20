# TechStore Analytics - Dashboard de Vendas 📊

## 🌐 Visão Geral

Este repositório contém o arquivo `tech.html`, que consiste em um **Dashboard de Vendas Interativo** (Single Page Application) desenvolvido para a empresa (fictícia/estudo) **TechStore**.

O painel foi construído com uma interface moderna (Dark Mode/Pro Level UI) e tem como foco a exibição clara de métricas comerciais e financeiras, permitindo que gestores e tomadores de decisão acompanhem o desempenho das vendas de forma ágil e visual.

## 🎯 Objetivo do Arquivo

O arquivo foi criado com o propósito central de **demonstrar habilidades em visualização de dados (Data Viz) e engenharia de front-end**. Ele simula o produto final de uma análise de Business Intelligence (BI), entregando:

1. **Autonomia ao usuário:** Capacidade de filtrar dados em tempo real sem precisar de recarregamento da página.

2. **Clareza Financeira:** Transformação de um banco de dados transacional em Indicadores-Chave de Desempenho (KPIs) diretos.

3. **Análise de Padrões:** Visualização da distribuição de vendas por categorias, canais e evolução temporal.

*(No contexto de um portfólio, este arquivo prova a capacidade do analista de ir além de ferramentas prontas como o Power BI, criando soluções personalizadas em HTML/JS).*

## ⚙️ Funcionalidades Principais

* **Filtros Dinâmicos:** Filtros em cascata por **Ano**, **Mês** e **Cidade** (Volta Redonda, Barra Mansa, Resende). Ao alterar um filtro, toda a tela é recalculada instantaneamente.

* **KPIs em Tempo Real:**

  * Faturamento Total
  * Lucro Bruto
  * Margem de Lucro (%)
  * Volume de Itens Vendidos

* **Gráficos Interativos (via Chart.js):**

  * **Gráfico de Barras:** Faturamento por Categoria de Produto (Notebooks, Celulares, Periféricos, Desktops).
  * **Gráfico de Rosca (Doughnut):** Participação de Vendas por Canal (E-commerce vs. Loja Física).
  * **Gráfico de Linha:** Curva de evolução do faturamento diário (com preenchimento e suavização).

## 💻 Tecnologias Utilizadas

O dashboard foi construído em um único arquivo de forma modular, garantindo fácil portabilidade e execução:

* **HTML5 & CSS3:** Estruturação semântica e estilização utilizando variáveis CSS (`:root`) para controle do Tema Escuro e sistema de grids responsivos (CSS Grid/Flexbox).
* **JavaScript (ES6+):** Lógica de ingestão de dados, processamento de arrays (`reduce`, `filter`, `map`) e atualização do DOM.
* [**Chart.js**](https://www.chartjs.org/): Biblioteca open-source em JavaScript utilizada para renderizar os gráficos de forma responsiva e animada.
* **Google Fonts:** Utilização da tipografia *Inter* para máxima legibilidade e design profissional.

## 🗄️ Estrutura de Dados

O sistema possui uma camada de "Ingestão Contínua" simulada. Os dados brutos (`rawData`) estão estruturados em formato JSON (Array de Objetos), contendo o histórico de pedidos de maio e junho de 2026. Essa estrutura foi pensada para ser facilmente substituída por uma API real (ex: `fetch('api/vendas')`) em futuras atualizações do projeto.

## 🚀 Como Executar Localmente

Este é um projeto *Client-Side* sem dependência de servidores complexos.

1. Faça o download do arquivo `tech.html`.
2. Dê um duplo clique no arquivo para abri-lo em qualquer navegador moderno (Chrome, Edge, Firefox, Safari).
3. É necessário possuir conexão com a internet apenas no primeiro acesso para que a biblioteca do Chart.js e a fonte do Google sejam carregadas via CDN.