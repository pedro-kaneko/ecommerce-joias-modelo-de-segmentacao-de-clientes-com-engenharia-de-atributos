![Google Colaboratory](https://img.shields.io/badge/Colab-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Numpy](https://img.shields.io/badge/Numpy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Scipy](https://img.shields.io/badge/Scipy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)

# 💍💎 eCommerce de Jóias | Modelo de Segmentação de Clientes com Engenharia de Atributos

### Relatório Interativo

Página web com o relatório do projeto, contendo análise detalhada e resultados da segmentação, além de gráficos interativos.

[![Relatório](https://img.shields.io/badge/HTML5-Relat%C3%B3rio%20Interativo-%23E34F26?style=flat&logo=HTML5&link=https%3A%2F%2Fpedro-kaneko.github.io%2Fecommerce-joias-modelo-de-segmentacao-de-clientes-com-engenharia-de-atributos%2F)](https://pedro-kaneko.github.io/ecommerce-joias-modelo-de-segmentacao-de-clientes-com-engenharia-de-atributos/)

### Notebook Python

Notebook do projeto, com o desenvolvimento completo e explicações técnicas detalhadas.

[![Kaggle Notebook](https://img.shields.io/badge/Kaggle-Jewellery_Customer_Segmentation_FeatureEngineering-blue?style=flat&logo=kaggle)](https://www.kaggle.com/code/pedrokaneko/jewellery-customer-segmentation-featureengineering)

# Introdução

Neste notebook, exploramos o conjunto de dados **"Customer Segmentation & Personas"**, uma base de dados de um e-commerce de joias, que inclui informações demográficas de clientes, comportamento de compra, tipos de produtos e métricas financeiras.

# Objetivo

O objetivo deste projeto é elaborar e implementar um modelo de segmentação de clientes com base em comportamento de compra, nível de interação com a marca e valor potencial para desenvolver estratégias de marketing mais personalizadas e eficientes.

# Resumo


Por meio da Análise Exploratória de Dados, foi identificado que 20% dos clientes se desligaram da empresa. Uma investigação mais detalhada supõe que algum fato ocorreu entre Outubro e Novembro de 2022, pois nesse período ocorreu uma inversão no fluxo de clientes. O processo de aquisições de clientes e início de assinaturas cessou e iniciou-se um processo de encerramento de assinaturas e a perda de clientes constantes, causando a diminuição gradual da base de clientes e, consequentemente, o rendimento da empresa. O evento ocorre de maneira abrangente, impactando todas as localidades que a empresa atua e todos os tipos de clientes.

O desenvolvimento de segmentação de clientes para direcionamento de campanhas de marketing surge como proposta de ação para contenção de danos, visando reter os clientes remanescentes e reativar os clientes desligados com estratégias direcionadas.

No processo de segmentação, os clientes tiveram um valor de importância atribuído através de uma métrica integrada (que considera aspectos diferentes) desenvolvida a partir da engenharia de atributos, formando grupos e segmentos distintos.

Insights relevantes podem ser gerados para cada um desses segmentos, como canal de venda mais efetivo, tipo de produto mais vendido, faixa etária e gênero predominantes. Da mesma maneira, cada segmento possui benchmarks únicos em relação a métricas como CPA, CLTV, tempo de retenção média.

Ao final, há um cálculo de payback, que indica o tempo necessário para recuperar o custo de aquisição de um cliente com base no valor que ele gera ao longo do tempo e o tempo médio de retenção, um ponto fundamental no planejamento.

# Conclusão

Este projeto visa a implementação de estratégias de segmentação de clientes mais precisas, baseadas em dados quantitativos, proporcionando um direcionamento mais eficaz para ações de marketing e potencializando o engajamento com a marca.

# Etapas

1. **Análise do Fluxo de Clientes e Financeira**
   - Verificação da proporção de clientes ativos e inativos.
   - Visualização da Receita por tipo de cliente e localidade.
2. **Identificação de Problemas**
   - Esgotamento da aquisição de clientes e início de assinaturas. 
   - Perda de clientes e encerramento de assinaturas constante em todas as localidades e tipos de cliente.
3. **Desenvolvimento de Soluções**
   - Proposta de segmentação de clientes para direcionamento de ações de marketing específicas como iniciativa de medida de contenção de danos.
4. **Segmentação de Clientes**
   - Desenvolvimento de estratégia de segmentação baseada em engenharia de atributos, utilizando as métricas RFM médio, Pontuação de Engajamento e CLTV.
   - Criação do indicador Valor Cliente (CustomerValueScore).
   - Criação da métrica categórica usada na segmentação: Grupos de Valor (CustomerValueGroup).
5. **Validação Estatística**
   - Verificando diferença estatística entre os segmentos de clientes formados.
6. **Campanhas de Marketing**
   - Desenvolvendo campanhas de marketing com objetivos específicos para cada segmento de cliente.
7. **Geração de Insights por Segmento (Clientes Ativos e Inativos)**
   - Tipos de produtos mais vendidos.
   - Canal de venda mais efetivo.
   - Faixa etária e gênero predominante.
   - CLTV, CPA e Tempo de retenção médio.
   - Payback por segmento (tempo necessário para recuperar valor investido).

# Metodologia

1. **Análise Exploratória de Dados (EDA)**  
   - **Análise Temporal**: Exploração de padrões sazonais, tendências e flutuações no fluxo de aquisição e perda de clientes ao longo do tempo, por meio de gráficos de séries temporais com frequência mensal e distribuições.
   - **Análise Financeira**: Visualização da receita, CPA, CLTV e tempo médio de retenção por tipo de cliente e localidade.  

2. **Análise Estatística**  
   - **Medidas de Dispersão**: Comparação de medidas de dispersão de variáveis-chave entre diferentes grupos de clientes e localidades utilizando box-plots.  

3. **Engenharia de Atributos (Feature Engineering)**  
   - **Normalização**: Normalização (MinMaxScaler) para padronizar métricas-chave (RFM médio, engajamento e CLTV) em uma escala comum.
   - **Definição dos Pesos**: Ponderação das métricas-chave (RFM médio, engajamento e CLTV) refletindo sua importância relativa no cálculo do novo indicador.
   - **Criação da Métrica Valor Cliente**: Criação da métrica CustomerValueScore elaborada pelo produto das três métricas-chave devidamente tratadas.
   - **Criação da Métrica Grupo de Valor**: Criação da métrica CustomerValueGroup a partir da transformação da métrica CustomerValueScore em métrica categórica.  

4. **Segmentação de Clientes**  
   - **Segmentação por Classificação**: Classificando os clientes de acordo com o seu grupo de valor atribuído.
   - **Análise Comparativa**: Comparação entre diferentes segmentos de clientes em termos de CLTV, engajamento e RFM médio, identificando padrões de comportamento e oportunidades de otimização.  

5. **Validação Estatística**  
   - **Teste de Levene**: Avaliação da homogeneidade das variâncias entre os segmentos antes da aplicação do teste ANOVA.
   - **Teste ANOVA (Padrão e Welch)**: Testando se há diferenças estatisticamente significativas entre segmentos de clientes em termos da métrica Valor Cliente.  

6. **Análise Descritiva**  
   - Gráficos interativos e tabelas de contingência para identificar padrões de cada segmento.  

# Conceito do Método de Segmentação Utilizado

Delegar a um modelo de clusterização a tarefa de segmentação de clientes pode simplificar o processo, no entanto há limitações consideráveis como falta de controle já que o modelo pode identificar padrões que não são relevantes para os objetivos e pode haver dificuldade de interpretação pois os padrões podem ser difíceis de explicar e relacionar com ações práticas. Assim, optamos por compreender e selecionar metricas de marketing específicas disponíveis e construir uma abordagem analítica controlada e direcionada.

<p>
$$
\text{ValorCliente} = (\overline{RFM} \times 0.3) \times (\text{ScoreEngajamento}_{\text{norm}} \times 0.4) \times (\text{CLTV}_{\text{norm}} \times 0.3)
$$
</p>


Através da engenharia de atributos integramos três métricas **RFM médio**, **Pontuação de Engajamento** e **CLTV** em um único indicador o **Valor Cliente** criando uma visão abrangente que integra do comportamentos de compra, capta níveis de interesse e envolvimento com a marca e potencial de geração de valor. E a partir desse indicador, criamos a uma métrica categórica **Grupo de Valor** que segmenta cada tipo de cliente (Standard, Engaged e Premium) em grupos de Valor (A, B e C).

# Conteúdo do Projeto

### Notebook Python

Notebook do projeto com explicação técnica e gráficos interativos:

[![Kaggle Notebook](https://img.shields.io/badge/Kaggle-Jewellery_Customer_Segmentation_FeatureEngineering-blue?style=flat&logo=kaggle)](https://www.kaggle.com/code/pedrokaneko/jewellery-customer-segmentation-featureengineering)

### Base de dados

A base de dados utilizada neste projeto está licenciada sob [MIT License](https://www.mit.edu/~amini/LICENSE.md).

[![Kaggle](https://img.shields.io/badge/Kaggle-Customer%20Segmentation%20and%20Personas-blue?style=flat&logo=kaggle)](https://www.kaggle.com/datasets/weihutchinson/customer-segementation-and-personas)

### Arquivo de requisitos:

Lista de bibliotecas e dependências necessárias para executar o projeto localmente.

[requirements.txt](https://github.com/pedro-kaneko/ecommerce-joias-modelo-de-segmentacao-de-clientes-com-engenharia-de-atributos/blob/main/requirements.txt)

# Como Utilizar

- **Kaggle:** Copie e edite diretamente no [Kaggle Notebook](https://www.kaggle.com/code/pedrokaneko/jewellery-customer-segmentation-featureengineering)
- **Localmente:** Faça o [Download](https://www.kaggle.com/kernels/scriptcontent/197976467/download) do notebook e da base de dados e execute no ambiente local. Instale as dependências listadas no [requirements.txt](https://github.com/pedro-kaneko/ecommerce-joias-modelo-de-segmentacao-de-clientes-com-engenharia-de-atributos/blob/main/requirements.txt)

---

**Autor:** Pedro Kaneko  
**Data:** [23/09/2024]
