# 📊 Projeto de Recuperação: Análise de Recursos Humanos (SQL & Python)

## 📌 Descrição do Projeto
Este projeto integra a extração de dados relacionais via **SQL (FreeSQL/Oracle - Esquema HR)** e a **Análise Exploratória de Dados (EDA) em Python**. O objetivo principal foi analisar o perfil remuneratório, a distribuição geográfica e o tempo de casa dos funcionários de uma organização para subsidiar tomadas de decisão em Gestão de Pessoas.

---

## 🗄️ Etapa 1: Consultas SQL (FreeSQL - Esquema HR)
Para a extração das bases de dados, foram construídas três consultas utilizando cláusulas de junção (`LEFT JOIN`), filtros e funções de extração de data:

1. **`query_01.csv` (Salários por Departamento e Cargo)**: Relaciona cada funcionário ao seu respectivo departamento e cargo, exibindo o salário atual ordenado por departamento e maior remuneração.
2. **`query_02.csv` (Distribuição Geográfica)**: Mapeia os funcionários conectando as tabelas de departamentos, localizações, países e regiões.
3. **`query_03.csv` (Admissão e Salários)**: Aplica a função `EXTRACT(YEAR FROM hire_date)` para isolar o ano de contratação e comparar com a evolução salarial dos colaboradores.

---

## 🐍 Etapa 2: Análise Estatística e Visualização (Python & Pandas)
Com os três arquivos `.csv` importados no Google Colab, realizou-se o diagnóstico estatístico da folha de pagamento e a geração de visualizações gráficas:

### 📈 Indicadores Salariais Principais:
- **Total de Funcionários Analisados**: 107 colaboradores.
- **Visualizações Geradas**:
  - **Histograma**: Distribuição da frequência salarial em faixas de remuneração.
  - **Gráfico de Colunas**: Média salarial agrupada por ano de admissão do funcionário.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
- **Banco de Dados**: Oracle SQL / FreeSQL (Esquema `HR`)
- **Linguagem de Programação**: Python 3
- **Bibliotecas Python**: Pandas, NumPy, Matplotlib
- **Ambiente de Desenvolvimento**: Google Colab
- **Versionamento & Documentação**: GitHub
