# Challenge-Telecom
Telecom X – Análise de Evasão de Clientes
Este projeto de Análise de Dados foi desenvolvido com o objetivo de investigar os motivos que levam à evasão (churn) de clientes em uma empresa fictícia de telecomunicações chamada Telecom X. Através de análise exploratória, visualizações, tratamento de dados e geração de insights, buscamos identificar os padrões que mais influenciam a saída dos clientes.
 
 Propósito do Projeto
A Telecom X enfrenta um alto índice de churn, o que compromete sua estabilidade financeira e crescimento. A proposta aqui é Compreender os fatores associados ao churn de clientes e propor recomendações estratégicas para a retenção.
O projeto foi estruturado com foco em clareza, replicabilidade e aplicabilidade prática, atendendo às exigências de um processo seletivo técnico.

Principais Insights
•	Contratos mensais estão altamente associados ao churn (44,5%).
•	Clientes com menor tempo de contrato e baixo custo diário apresentam maior evasão.
•	Débito eletrônico é o método de pagamento mais usado entre churners.
•	A maior evasão está nos primeiros meses de contrato e entre clientes que contratam serviços digitais, como streaming e internet.
•	Idosos, solteiros e sem dependentes são perfis mais frequentes entre os que cancelam.

Estrutura do Projeto
Telecom_X/
├── README.md → Este arquivo
├── Relatorio_Telecom.docx → Relatório final com achados e recomendações
├── Final_de_challenge_telecon.py → Script completo da análise (Colab/IPYNB convertido)
├── graficos/
│ ├── grafico_ Clientes por faixa de Custo diário e status de churn.png
│ ├── grafico_ Distribuição de Churn por Característica Pessoal.png
│ ├── grafico_ Distribuição de Churn por Gênero.png
│ ├── grafico_ Distribuição de Churn por Método de Pagamento.png
│ ├── grafico_ Distribuição de Churn por Tipo de Contrato.png
│ ├── grafico_ Distribuição de Clientes por Churn.png
│  └── grafico_ Distribuição de evasão de clientes por método de pagamento.png
|    └── grafico_ Evasão por faixa de gasto total.png
|    └── grafico_ Quantidade de churners por serviço utilizado.png
|    └── grafico_ Churn por Tempo de Contrato.png
└── scripts/
└── gerar_graficos.png → Script com funções de visualização salvas

Exemplos de Gráficos
 Tipo de Contrato x Churn
<img src=’graficos/grafico_Distribuição de Churn por Tipo de Contrato.png’>
- Contrato mensal = alta evasão | Contrato bianual = alta retenção.

Tempo de x Evasão
<img src=’graficos/grafico_ Churn por Tempo de Contrato.png’>
- A evasão cai drasticamente após 10 meses de permanência**.

Distribuição de Clientes por Churn 
- <img src=’graficos/ grafico_ Distribuição de Clientes por Churn.png ‘>
 28,8% dos clientes cancelaram seus contratos.

Churn por Gênero
<img src=’graficos/grafico_ Distribuição de Churn por Gênero.png’>
Homens (29%) e mulheres (28,5%) apresentam proporções semelhantes de evasão .

Churn por Tipo de Contrato
<img src=’graficos/grafico_Distribuição de Churn por Tipo de Contrato.png’>
- Contrato mensal = alta evasão (44%) | Contrato bianual = alta retenção (5,5%).
 
Churn por Característica Pessoal
<img src=’graficos/grafico_ Distribuição de Churn por Característica Pessoal.png’>
Idosos, solteiros e sem dependentes aparecem mais entre os evasores
 
Churn por Método de Pagamento
<img src=’graficos/grafico_ Distribuição de Churn por Método de Pagamento.png’>
 
Distribuição de evasão de clientes por método de pagamento
<img src=’graficos/grafico_ de evasão de clientes por método de pagamento.png’>
Clientes que usam **débito eletrônico têm maior probabilidade de churn.
 
Evasão por gasto total
<img src=’graficos/grafico_ Evasão por faixa de gasto total.png’>
Quanto menor o gasto total, maior a evasão
 
Evasão por gasto diário
<img src=’graficos/grafico_ Clientes por faixa de Custo diário e status de churn.png’>
 
Quantidade de Churners por serviço utilizado
<img src=’graficos/grafico_ Quantidade de churners por serviço utilizado.png’>
Os serviços de internet tem a maior evasão
 
Tempo de Contrato
<img src=’graficos/grafico_ Churn por Tempo de Contrato.png’>
A evasão cai drasticamente após 10 meses de permanência  

Como Executar este Projeto
Requisitos
- Python 3.8+
- Bibliotecas: `pandas`, `numpy`, `matplotlib`, `scipy`

Instalação
Clone este repositório:
git clone https://github.com/haydeemagrina/telecom-x-churn-analysis.git
cd telecom-x-churn-analysis

 Instale as dependências (recomenda-se usar um ambiente virtual):
pip install pandas matplotlib numpy

Execute o notebook:
•	Abra o Jupyter Notebook ou Google Colab.
•	Carregue o arquivo: final_de_challenge_telecon.ipynb.
•	Siga as células sequencialmente.

Etapas Realizadas
1. Limpeza e Tratamento dos Dados
•	Normalização de colunas aninhadas (phone, internet, account)
•	Conversão de variáveis categóricas para booleanas
•	Tratamento de valores ausentes e não numéricos (ex: Charges.Total)
•	Criação de variáveis novas como Custo Diário e Faixa de Gasto
2. Análise Exploratória (EDA)
•	Comparações por gênero, tipo de contrato, idade, método de pagamento, etc.
•	Visualizações com gráficos de pizza, barras e linha
•	Criação de faixas para análise de churn por gasto e tempo
3. Conclusões e Recomendações
•	Estratégias para retenção com base em dados objetivos
•	Segmentação de clientes em risco e propostas de ação

Possíveis Extensões
•	Implementar modelo preditivo de churn (ex: Random Forest ou XGBoost)
•	Dashboards interativos com Streamlit ou Power BI

Autor: Projeto desenvolvido por Haydée Magriñá como parte de um desafio de análise de dados.
Contato: [haydeemagrina@gmail.com]
 
