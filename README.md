# 📊 Projeto de Análise de Salários na Área de Dados

Este projeto consiste em uma análise completa de dados sobre cargos e salários na área de tecnologia e dados ao redor do mundo. O objetivo é explorar tendências de mercado, faixas salariais por senioridade e o impacto do trabalho remoto, culminando em um dashboard interativo.

## 🗂️ Estrutura do Projeto

O projeto está dividido em duas etapas principais:
1. **Análise e Tratamento de Dados (`Carlos_Daniel.ipynb`)**: Processamento dos dados brutos.
2. **Dashboard Interativo (`app.py`)**: Apresentação dos resultados via Streamlit.

---

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Manipulação de Dados:** Pandas
* **Visualização:** Plotly Express
* **Dashboard:** Streamlit
* **Ambiente de Desenvolvimento:** Jupyter Notebook / Google Colab / Vs Code

---

## 🚀 Etapa 1: Coleta e Tratamento de Dados (ETL)

No arquivo `Carlos_Daniel.ipynb`, foi realizado o processo de limpeza e preparação da base de dados original (`salaries.csv`). As principais etapas incluíram:

* **Tradução e Renomeação:** Conversão dos nomes das colunas e dos valores categóricos do inglês para o português para facilitar a análise (ex: `work_year` para `ano`, `FT` para `Tempo Integral`).
* **Mapeamento de Dados:**
    * **Senioridade:** Senior, Pleno, Júnior e Executivo.
    * **Modelo de Trabalho:** Presencial, Remoto e Híbrido.
    * **Porte da Empresa:** Pequeno, Médio e Grande.
* **Limpeza de Dados:** Identificação e remoção de registros nulos (linhas sem informação de ano).
* **Conversão de Tipos:** Ajuste de tipos de dados (ex: conversão da coluna `ano` para inteiro) para garantir a precisão nos filtros e gráficos.
* **Exportação:** Os dados tratados foram preparados para alimentar o dashboard.

---

## 📊 Etapa 2: Dashboard Interativo

O arquivo `app.py` contém o código do dashboard desenvolvido com **Streamlit**. Ele consome os dados tratados (hospedados no repositório) e oferece uma interface amigável para exploração.

### Funcionalidades do Dashboard:
* **Filtros Dinâmicos:** Barra lateral ("🔍 Filtros") que permite selecionar dados específicos por:
    * Ano
    * Nível de Senioridade
    * Tipo de Contrato
* **Visualização de Dados:** Gráficos interativos gerados com **Plotly** que respondem aos filtros aplicados, permitindo uma análise granular dos salários em dólares (USD).

---

## 🏁 Como Executar o Projeto

1. Clone este repositório:
   ```bash
   https://relatorio-data-scientist.streamlit.app/
