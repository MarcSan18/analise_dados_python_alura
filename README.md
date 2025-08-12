# 📊 Imersão de Dados com Python e IA

Análise exploratória de salários em cargos de dados.

Este projeto realiza uma análise exploratória de um dataset contendo informações sobre salários em diversas áreas de dados. O objetivo é entender as tendências de salários, os fatores que os influenciam (como nível de experiência, tipo de emprego, localização, etc.) e fornecer insights sobre o mercado de trabalho em dados.

---

## 🛠️ Ferramentas e Bibliotecas Utilizadas

Nesta análise, foram utilizadas as seguintes ferramentas e bibliotecas Python:

- **Pandas**: Manipulação e análise de dados, leitura do CSV, limpeza, transformação, agrupamento e estatísticas descritivas.
- **Matplotlib**: Criação de visualizações estáticas como gráficos de barras e histogramas.
- **Seaborn**: Visualizações estatísticas mais atraentes, como box plots.
- **Plotly Express**: Gráficos interativos e dinâmicos, incluindo mapa coroplético.
- **pycountry**: Conversão de códigos de país ISO-2 para ISO-3, necessário para o mapa coroplético.

---

## 📁 Dados

O dataset utilizado neste projeto é o `salaries.csv`, obtido do repositório [data-jobs/salaries.csv](https://raw.githubusercontent.com/guilhermeonrails/data-jobs/refs/heads/main/salaries.csv). Ele contém as seguintes colunas:

| Coluna                | Descrição                                                                 |
|----------------------|---------------------------------------------------------------------------|
| `ano_trabalho`       | Ano em que o trabalho foi realizado                                       |
| `nivel_experiencia`  | Nível de experiência do profissional (Júnior, Pleno, Sênior, Executivo)   |
| `tipo_emprego`       | Tipo de contrato de trabalho (Tempo Integral, Contrato, etc.)             |
| `cargo`              | Cargo do profissional                                                     |
| `salario`            | Salário na moeda local                                                    |
| `moeda_salario`      | Moeda do salário                                                          |
| `salario_em_usd`     | Salário convertido para dólares americanos (USD)                          |
| `residencia_empregado` | País de residência do empregado                                         |
| `taxa_remoto`        | Percentual de trabalho remoto (0, 50, 100)                                |
| `localizacao_empresa`| País da sede da empresa                                                   |
| `tamanho_empresa`    | Tamanho da empresa (Pequena, Média, Grande)                               |

---

## 📈 Análise Realizada

As seguintes etapas foram realizadas neste notebook:

1. **Carregamento dos Dados**: Dataset carregado em um DataFrame pandas.
2. **Exploração Inicial**: Visualização geral com `head()`, `info()`, `describe()` e `shape`.
3. **Tradução de Colunas**: Nomes das colunas traduzidos para português.
4. **Tradução de Categorias**: Tradução das categorias de senioridade, contrato, tamanho da empresa e remoto.
5. **Verificação de Valores**: Distribuição de valores em colunas categóricas com `.value_counts()`.
6. **Tratamento de Valores Ausentes**: Remoção de linhas com valores ausentes na coluna 'ano'.
7. **Conversão de Tipo de Dado**: Conversão da coluna 'ano' para inteiro.
8. **Distribuição de Senioridade**: Gráfico de barras da distribuição dos níveis de senioridade.
9. **Salário por Senioridade**: Gráficos de barras, box plots e gráficos interativos com Plotly.
10. **Salário para Data Scientists por País**: Gráfico interativo e mapa coroplético com Plotly e pycountry.
11. **Proporção de Tipos de Trabalho**: Gráficos de pizza com Plotly.
12. **Salvando o DataFrame Limpo**: Exportação do `df_limpo` para CSV como `dados_final_imersão_alura.csv`.

---

## ✅ Conclusão

Esta análise inicial forneceu insights valiosos sobre os salários em cargos de dados, destacando a influência do nível de senioridade e a variação salarial entre diferentes países.

---

## 🔍 Próximos Passos

Para aprofundar a análise, sugerimos:

- Analisar a distribuição dos salários por tipo de emprego e tamanho da empresa.
- Investigar a relação entre taxa de trabalho remoto e salário.
- Realizar uma análise temporal da evolução salarial.
- Explorar os cargos mais comuns e seus respectivos salários.
- Realizar uma análise de correlação entre variáveis numéricas.
