# 📊 Transformação, Conversão e Agrupamento de Dados com K-Means

Projeto prático desenvolvido para a disciplina de Data Science, com o objetivo de realizar o pipeline completo de engenharia de dados e modelagem não supervisionada em uma base de clientes fictícia.

---

## 🛠️ Tecnologias e Ferramentas Utilizadas
* **Python** (Google Colab)
* **Pandas & NumPy** (Manipulação e limpeza de dados)
* **Matplotlib** (Visualização e gráficos estatísticos)
* **Scikit-Learn** (Pré-processamento, K-Means Clustering, Pipelines e Train-Test Split)

---

## 🔍 Etapas do Projeto
1. **Inspeção de Dados:** Análise estrutural de tipos (`info()`, `describe()`), contagem de valores nulos e identificação de inconsistências em variáveis categóricas.
2. **Limpeza e Conversão:** Tratamento de colunas monetárias (`renda_mensal`, `gasto_mensal`), extração de idades numéricas, padronização de datas (datetime) e tratamento de valores ausentes pela mediana.
3. **Codificação (Encoding):** Aplicação de codificação ordinal para escolaridade e *One-Hot Encoding* para variáveis geográficas (`cidade`).
4. **Transformação de Variáveis:** Análise de distribuição via histogramas, aplicação de transformação logarítmica (`log1p`), discretização (`pd.cut` e `pd.qcut`) e criação de métricas derivadas.
5. **Normalização e Escalonamento:** Comparação detalhada entre `MinMaxScaler` e `StandardScaler`, avaliando o comportamento frente a *outliers*.
6. **Agrupamento (K-Means):** Execução do algoritmo de clusterização com $k=3$ comparando cenários com e sem dados escalonados, evidenciando o impacto da escala das variáveis.
7. **Boas Práticas de Engenharia:** Divisão de bases de dados (`train_test_split`) prevenindo vazamento de dados (*data leakage*) e construção de um `Pipeline` automatizado no Scikit-Learn.
