# DP-900: Microsoft Azure Data Fundamentals

## Módulo 4: Explore a análise moderna de data warehouse

- **Objetivos módulo 4:**
  1. Examinar os componentes de um data warehouse moderno;
  2. Explorar analise de dados em larga escala;
  3. Comece a criar com o Power BI.
  
### Unidade 1: Examinar os componentes de um data warehouse moderno

- **Objetivos da unidade 1:**
  1. Explorar conceitos de data warehousing(grande armazenamento, estoque de dados);
  2. Explorar os Servicos de Dados do Azure para um data warehousing moderno;
  3. Explorar uma arquitetura e uma carga de trabalho de data warehousing moderno;
  4. Explorar os Servigos de Dados do Azure no portal do Azure.

- **Componentes do data warehouse moderno:**

  - Modelo de arquitetura em três camadas:
  
  ![image](https://user-images.githubusercontent.com/86172286/189776732-3ec80bde-f5c4-431e-bb74-7cb245cc17e7.png)

  - Onde temos os dados sendo injeridos através de um processo de ingestâo. Que pode vir de diversas fontes: Banco realacional, arquivos em pastas, planilhas. E o `Azure Data Factory` injere esses dados recebidos, transforma, limpa, faz um processo de `ETL`(Extract, transform, load/Extrair, transformar e carregar) deixa todos os dados no mesmo formato e armazena eles em um `Data Lake`(pode ser o Data Lake Storage, por exemplo):

  ![1](https://user-images.githubusercontent.com/86172286/189778388-e6d59485-c4ed-4b29-b623-c0c9fcc01c6b.png)

  - Depois disso, temos dois caminhos:
    1. Seguir diretamente para o `Synapse Services` onde ele irá fazer um trabalho de normalização dos dados, limpeza, armazenar e entregar os dados.
    2. Ou seguir com esses dados para o `Databricks`, onde podemos fazer análise cognitiva, limpar os dados, e trabalhar os dados. E depois usar o `Synapse` como um Hub para armazenar os dados para entregar os dados para o `Analise Services`.

   ![1](https://user-images.githubusercontent.com/86172286/189778997-99a92f2b-5903-4979-aded-6259510904ac.png)

  - No `Analise Services` será feito o tratamento dos dados para gerar os insights combinados com o negócio e expor os dados para o `Power BI` consumir:

   ![1](https://user-images.githubusercontent.com/86172286/189779621-0f996770-c4df-4ac5-ac2a-a4e7a05373ca.png)

  - Todo esse processo é categorizado em três camadas:
    1. **Bronze:** Nessa camada o dado ainda não tem tanto valor;
    2. **Prata:** Nessa camada o dado já tem um valor por já está trabalhado, mas não tem o valor total;
    3. **Ouro:** Nessa camada o dado já está tratado, limpo, pronto para ser consumido e gerar retornos/insights para o negócio.

    ![image](https://user-images.githubusercontent.com/86172286/189779910-f0def067-ddcc-4b4c-9f4b-786f90f85b9b.png)
    
 - **Servicos de Dados do Azure para um data warehousing moderno:**

  1. **Azure Data Factory:**
  2. **Azure Data Lake:**
  3. **Azure Databricks:**
  4. **Azure HDInsight:**
  5. **Azure Synapse Análise:**
  

  ![image](https://user-images.githubusercontent.com/86172286/189780107-5481bf7b-b753-4ad9-8fc2-632c382607ab.png)


### Unidade 1: Verificação de conhecimento


