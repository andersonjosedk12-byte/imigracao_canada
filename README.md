# 🇨🇦 Projeto de Portfólio: Visualização de Dados de Imigração (Canadá)

Este projeto documenta uma análise exploratória e a construção de visualizações para dados de imigração no Canadá (1980–2013). O notebook `Aula_5.ipynb` parte de um arquivo CSV (`imigrantes_canada.csv`), organiza a base e cria gráficos com **Matplotlib**, **Seaborn** e **Plotly**, com foco em **legibilidade**, **storytelling** e **exportação** de artefatos (PNG/HTML).

## 🚀 Funcionalidades

- Carregamento e validação do dataset (`imigrantes_canada.csv`) com fallback para execução local/Colab.
- Preparação dos dados para séries temporais (lista de anos `1980–2013`, indexação por país).
- Extração de recortes de análise (ex.: série do **Brasil** e países da **América do Sul**).
- Criação de gráficos estáticos com **Matplotlib**:
  - Linhas (tendência temporal)
  - Barras (comparação por total)
  - Boxplot (distribuição/variabilidade)
  - Subplots (comparação entre países)
- Refinamento visual e storytelling:
  - Ajustes de tamanho, título, rótulos e ticks
  - Grid, espessura de linha, marcadores
  - Destaque do Brasil no ranking (cores + ordenação)
  - Anotações com valores nas barras
  - Limpeza de ruído visual (remoção de frame/ticks/eixos)
- Visualizações interativas com **Plotly** (exploração por hover, zoom, legenda).
- Exportação de gráficos:
  - PNG (Matplotlib)
  - HTML (Plotly)

## 📈 Principais análises

O notebook enfatiza dois recortes:

- **Brasil (1980–2013)**: tendência temporal e distribuição (inclui descritivo/boxplot).
- **América do Sul (1980–2013)**: comparação do total acumulado por país, ranking ordenado e destaque do Brasil.

> Observação: os “insights finais” do estudo estão consolidados em uma seção no final do notebook.

## 🧱 Pipeline do Notebook

1. **Entendimento do conjunto de dados** – carga, inspeção e preparação das colunas de anos.
2. **Série do Brasil** – extração e criação de DataFrame para visualização temporal.
3. **Matplotlib: primeiros gráficos** – plot básico, `xticks/yticks`, `figure`, títulos e rótulos.
4. **Matplotlib: subplots** – comparação (Brasil, Colômbia, Argentina, Peru) e padronização de escalas.
5. **Refinamento visual e storytelling** – estilo, grid, cores, destaque do Brasil e anotações.
6. **Exportação** – salvar gráficos em PNG e exportar visualizações interativas em HTML.
7. **Insights (principais achados)** – síntese dos resultados observados.

## 🛠️ Tecnologias Utilizadas

- Python 3.9+
- Pandas
- Matplotlib
- Seaborn
- Plotly
- Jupyter Notebook / Google Colab

## ▶️ Como Executar

1. **Garanta os arquivos na pasta do projeto**:
   - `Aula_5.ipynb`
   - `imigrantes_canada.csv`

2. **Instale dependências**:
   ```bash
   pip install pandas matplotlib seaborn plotly
   ```

3. **Abra o notebook**:
   ```bash
   jupyter notebook "Aula_5.ipynb"
   ```

4. **Execute as células em ordem**.

## 📁 Estrutura do Projeto

- `Aula_5.ipynb` – notebook principal (pipeline + gráficos + insights)
- `imigrantes_canada.csv` – dataset base
- `imigracao_brasil_canada.png` – exemplo de exportação (Matplotlib)
- `imigracao_america_sul.png` – exemplo de exportação (Matplotlib)
- `imigracao_america_sul.html` – exemplo de exportação interativa (Plotly)

## 🔍 Principais aprendizados

1. A **ordenação** (ranking) e o **destaque por cor** tornam comparações muito mais imediatas.
2. Subplots com **mesma escala** evitam interpretações incorretas ao comparar países.
3. Visualização interativa (Plotly) complementa a análise: permite explorar detalhes sem poluir o gráfico.
4. Pequenos ajustes (ticks, grids, remoção de frames) elevam bastante a qualidade do gráfico para portfólio.

## 📝 Licença

Projeto distribuído sob licença MIT.
