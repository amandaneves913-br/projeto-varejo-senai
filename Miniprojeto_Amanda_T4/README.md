# Mini-Projeto Avaliativo - Módulo 1 (Varejo)

## 📋 Instruções de Execução
1. Certifique-se de ter o Python e a biblioteca **Pandas** instalados no seu ambiente (VS Code ou Google Colab).
2. Faça o download da base de dados `Base Varejo.csv` (ou da amostra tratada) e do script em Python.
3. Abra o arquivo de código em sua IDE de preferência e execute todas as células para realizar a Análise Exploratória de Dados (AED).

---

## 🧠 Reflexão Teórica: ETL e Qualidade de Dados
O processo de **ETL (Extract, Transform, Load)** é fundamental na engenharia e análise de dados. 
* **Extração (Extract):** Consiste em coletar os dados brutos de fontes diversas (neste caso, a base de varejo).
* **Transformação (Transform):** Etapa vital onde garantimos a qualidade dos dados — lidando com valores nulos (preenchendo categorias ausentes), eliminando duplicatas indesejadas e convertendo tipos de dados (como transformar colunas de texto de data em objetos reais do tipo `datetime`). Dados limpos evitam distorções em futuras análises de Business Intelligence.
* **Carga (Load):** Salvamento da base tratada pronta para alimentar dashboards ou análises avançadas.

---

## 💡 Principais Insights Obtidos
1. **Concentração de Vendas por Categoria:** A categoria **Alimentos** lidera expressivamente o volume de compras na base, representando a grande maioria das transações registradas.
2. **Perfil Demográfico (Filhos):** A análise estatística da coluna de número de filhos (`CL_FHL`) apontou que a mediana e a moda são iguais a **0**, indicando que a maior parte dos clientes compradores não possui filhos cadastrados.
3. **Distribuição por Gênero:** O volume de compras apresentou um perfil equilibrado entre os gêneros, com uma leve predominância de registros associados ao público feminino.
4. **Importância da Limpeza de Dados:** A identificação de registros sem categoria (`#N/D`) reforçou a necessidade de tratamentos condicionais prévios para evitar falhas em agrupamentos futuros (`groupby`).
