# Imersão de dados com Python e IA

Análise Exploratoria de Salários em Cargos de Dados.

Análise de Salários em Cargos de Dados

Este projeto realiza uma análise exploratória de um dataset contendo informações sobre salários em diversas áreas de dados. O objetivo é entender as tendências de salários, os fatores que os influenciam (como nível de experiência, tipo de emprego, localização, etc.) e fornecer insights sobre o mercado de trabalho em dados.

Dados
O dataset utilizado neste projeto é o salaries.csv, obtido do repositório https://raw.githubusercontent.com/guilhermeonrails/data-jobs/refs/heads/main/salaries.csv. Ele contém as seguintes colunas:

ano_trabalho: Ano em que o trabalho foi realizado.
nivel_experiencia: Nível de experiência do profissional (Júnior, Pleno, Sênior, Executivo).
tipo_emprego: Tipo de contrato de trabalho (Tempo Integral, Contrato, Tempo Parcial, Freelancer).
cargo: Cargo do profissional.
salario: Salário na moeda local.
moeda_salario: Moeda do salário.
salario_em_usd: Salário convertido para dólares americanos (USD).
residencia_empregado: País de residência do empregado.
taxa_remoto: Percentual de trabalho remoto (0, 50, 100).
localizacao_empresa: País da sede da empresa.
tamanho_empresa: Tamanho da empresa (Pequena, Média, Grande).
Análise Realizada
Até o momento, as seguintes etapas foram realizadas neste notebook:

Carregamento dos Dados: O dataset foi carregado em um DataFrame pandas.
Exploração Inicial: Foram verificadas as primeiras linhas do DataFrame (df.head()), informações gerais (df.info()), estatísticas descritivas (df.describe()) e as dimensões do dataset (df.shape).
Tradução de Colunas: Os nomes das colunas foram traduzidos para português brasileiro.
Tradução de Categorias: As categorias das colunas senioridade, contrato, tamanho_empresa e remoto foram traduzidas para português.
Verificação de Valores: A distribuição dos valores em algumas colunas categóricas foi verificada (.value_counts()).
Tratamento de Valores Ausentes: As linhas com valores ausentes na coluna 'ano' foram removidas, criando um novo DataFrame df_limpo.
Conversão de Tipo de Dado: A coluna 'ano' no DataFrame df_limpo foi convertida para o tipo inteiro.
Próximos Passos
Algumas sugestões para continuar a análise incluem:

Analisar a distribuição dos salários (salario_em_usd) por diferentes categorias (nível de experiência, tipo de emprego, localização, etc.).
Visualizar as principais descobertas utilizando gráficos (histogramas, box plots, gráficos de barras, etc.).
Investigar a relação entre a taxa de trabalho remoto e o salário.
Analisar a evolução dos salários ao longo dos anos.
Explorar os cargos mais comuns e seus respectivos salários.
Este README será atualizado conforme a análise progredir.
