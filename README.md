# Telecom X - Análise de Evasão de Clientes (Churn)

![Status do Projeto](https://img.shields.io/badge/Status-Concluído-brightgreen)

## 📖 Descrição do Projeto

Este projeto consiste em uma **Análise Exploratória de Dados (EDA)** realizada sobre um conjunto de dados da empresa fictícia "Telecom X". A empresa enfrenta um alto índice de evasão de clientes (churn) e o objetivo desta análise é identificar os principais fatores e perfis de clientes que estão mais propensos a cancelar seus serviços.

Os insights gerados aqui servem como base para a tomada de decisão estratégica e para o desenvolvimento de modelos de *machine learning* para prever o churn de clientes em fases futuras do projeto.

## 🚀 O Desafio

O desafio proposto foi atuar como analista de dados para:
1.  **Coletar e tratar os dados** de uma fonte externa (API/JSON).
2.  **Aplicar os conceitos de ETL** (Extração, Transformação e Carga) para preparar os dados para análise.
3.  **Realizar uma Análise Exploratória de Dados (EDA)** completa e gerar insights relevantes.
4.  **Criar visualizações de dados estratégicas** para identificar padrões e tendências.
5.  **Comunicar os resultados** de forma clara e objetiva.

## 📊 Fonte de Dados

Os dados foram extraídos de um arquivo JSON hospedado no GitHub, contendo informações demográficas, de contrato, serviços contratados e financeiras sobre os clientes da Telecom X.

* **URL dos dados:** [TelecomX_Data.json](https://raw.githubusercontent.com/ingridcristh/challenge2-data-science/main/TelecomX_Data.json)

## 🛠️ Ferramentas e Bibliotecas

O projeto foi desenvolvido inteiramente em Python, utilizando o ambiente do Google Colab. As principais bibliotecas utilizadas foram:

* **`requests`**: Para realizar a requisição HTTP e extrair os dados da fonte.
* **`pandas`**: Para manipulação, limpeza e estruturação dos dados.
* **`matplotlib`**: Para a criação de gráficos base.
* **`seaborn`**: Para a criação de visualizações estatísticas mais elaboradas e esteticamente agradáveis.

##  workflow Estrutura do Projeto

A análise foi estruturada seguindo as melhores práticas de um projeto de ciência de dados:

1.  **Extração, Transformação e Carga (ETL)**: Conexão com a fonte de dados, normalização da estrutura JSON aninhada, limpeza de dados (tratamento de valores nulos e conversão de tipos), e preparação do dataset para análise.
2.  **Análise Exploratória de Dados (EDA)**: Investigação profunda das variáveis para entender suas distribuições e relações com a variável alvo (`Churn`).
3.  **Engenharia de Atributos**: Criação de novas variáveis (`Contas_Diarias`) para enriquecer a análise.
4.  **Análise de Correlação**: Uso de um mapa de calor (heatmap) para visualizar a correlação entre as variáveis numéricas.
5.  **Geração de Insights e Conclusões**: Sumarização dos achados em um relatório final.

## 📈 Principais Insights e Conclusões

A análise revelou padrões claros sobre o perfil dos clientes que tendem a cancelar o serviço:

* **Tipo de Contrato é Crucial**: Clientes com **contrato mensal** têm uma taxa de churn drasticamente maior em comparação com contratos de 1 ou 2 anos.
* **Clientes Novos são Vulneráveis**: A evasão é significativamente maior nos **primeiros meses de serviço**. Clientes com baixo tempo de casa (`tenure`) são o principal grupo de risco.
* **Preço Importa**: Clientes com **taxas mensais mais altas** apresentam maior propensão ao churn, especialmente aqueles com serviço de Fibra Óptica, sugerindo uma possível sensibilidade ao preço ou problemas de qualidade/percepção de valor.
* **Serviços de Proteção Retêm Clientes**: Clientes sem serviços de valor agregado como `SegurancaOnline` e `BackupOnline` cancelam com muito mais frequência.
* **Forma de Pagamento**: O pagamento via **cheque eletrônico** está associado a uma taxa de churn notavelmente mais alta.

## 🔮 Próximos Passos

Com base nesta análise exploratória, os próximos passos recomendados são:
1.  **Pré-processamento avançado**: Codificar variáveis categóricas (One-Hot Encoding) e escalar as variáveis numéricas.
2.  **Construção de Modelos Preditivos**: Desenvolver e treinar modelos de machine learning (ex: Regressão Logística, Random Forest, Gradient Boosting) para prever a probabilidade de churn para cada cliente.
3.  **Avaliação e Interpretação do Modelo**: Utilizar métricas como Acurácia, Precisão, Recall e AUC ROC para avaliar o melhor modelo e analisar a importância das features (`feature_importance_`) para confirmar os achados da EDA.

## 🚀 Como Executar o Projeto

Para replicar esta análise, siga os passos abaixo:

1.  **Clone o repositório:**
    ```bash
    git clone [https://github.com/seu-usuario/nome-do-repositorio.git](https://github.com/seu-usuario/nome-do-repositorio.git)
    ```
2.  **Navegue até o diretório do projeto:**
    ```bash
    cd nome-do-repositorio
    ```
3.  **Instale as dependências:** (Crie um arquivo `requirements.txt` com o conteúdo abaixo)
    ```
    pandas
    requests
    matplotlib
    seaborn
    ```
    Execute o comando:
    ```bash
    pip install -r requirements.txt
    ```
4.  **Execute o notebook**: Abra o arquivo `.ipynb` (por exemplo, `analise_churn.ipynb`) em um ambiente como Jupyter Notebook, Jupyter Lab ou Google Colab e execute as células na ordem.

## 👨‍💻 Autor

Projeto desenvolvido por **Thiago Alencar** como parte de um desafio de Análise de Dados.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/thiago-alencar-antonio/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Thiago-Alencar/)
