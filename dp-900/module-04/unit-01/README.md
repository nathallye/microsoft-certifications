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

  - Onde temos os dados sendo injeridos através de um processo de ingestâo. Que pode vir de diversas fontes: Banco realacional, arquivos em pastas, planilhas. E o `Azure Data Factory` injere esses dados recebidos, transforma, limpa, faz um processo de `ETL`(Extract, transform, load/Extrair, transformar e carregar) deixa todos os dados no mesmo formato e armazena eles em um `Data Lake`(pode ser o Data Lake Storage, por exemplo), esses dados ainda são brutos:

  ![1](https://user-images.githubusercontent.com/86172286/189778388-e6d59485-c4ed-4b29-b623-c0c9fcc01c6b.png)

  - Depois disso, temos dois caminhos:
    1. Seguir diretamente para o `Synapse Services` onde ele irá fazer um trabalho de normalização dos dados, limpeza, armazenar e entregar os dados.
    2. Ou seguir com esses dados para o `Databricks`, onde podemos fazer análise cognitiva, limpar os dados, e trabalhar os dados. E depois usar o `Synapse` como um Hub para armazenar os dados para entregar os dados para o `Analise Services`.

   ![1](https://user-images.githubusercontent.com/86172286/189778997-99a92f2b-5903-4979-aded-6259510904ac.png)

  - No `Analise Services` será feito o tratamento dos dados para gerar os insights combinados com o negócio e expor os dados para o `Power BI` consumir:

   ![1](https://user-images.githubusercontent.com/86172286/189784705-aa4aa2dd-a3cf-491c-b82e-9cf0fec344bd.png)

  - Todo esse processo é categorizado em três camadas:
    1. **Bronze:** Nessa camada o dado ainda não tem tanto valor;
    2. **Prata:** Nessa camada o dado já tem um valor por já está trabalhado, mas não tem o valor total;
    3. **Ouro:** Nessa camada o dado já está tratado, limpo, pronto para ser consumido e gerar retornos/insights para o negócio.

    ![image](https://user-images.githubusercontent.com/86172286/189779910-f0def067-ddcc-4b4c-9f4b-786f90f85b9b.png)
    
 - **Servicos de Dados do Azure para um data warehousing moderno:**
  1. **Azure Data Factory:** Serviço que podemos trabalhar com a parte de ingestão de dados e processo de `ETL`. Componentes importantes -> `Datasets` onde cada dataset representa uma tabela ou um conjunto de dados e a `pipeline`(a segmentação de instruções é uma técnica de hardware que permite que a CPU realize a busca de uma ou mais instruções além da próxima a ser executada).
  2. **Azure Data Lake:** Serviço de armazenamento, podemos trabalhar com o Data Lake Store e o Data Lake Storege(com namespace hierarquico habilitado).
  3. **Azure Databricks:** Ferramenta parecida com o `Azure Synapse Analytics`, ambas trabalham baseadas em apache spark(ferramenta como base de processamento). Trabalha com fluxo de dados gerando no final do fluxo armazenando os arquivois tratados em uma tabela virtual ou uma view. Streaming de big data, processamento em tempo real.
  4. **Azure HDInsight:** Serviço baseado em hadoop(plataforma de software em Java de computação distribuída voltada para clusters e processamento de grandes volumes de dados, com atenção a tolerância a falhas. Foi inspirada no MapReduce e no GoogleFS). Serve para processar grandes volumes de big data.
  5. **Azure Synapse Analytics:** Baseada em apache spark(ferramenta como base de processamento). Trabalha com fluxo de dados gerando no final do fluxo armazenando os arquivois tratados em uma tabela virtual ou uma view. Trabalha com o banco de dados SQL por trás.

  ![image](https://user-images.githubusercontent.com/86172286/189780107-5481bf7b-b753-4ad9-8fc2-632c382607ab.png)
  
  - **O que é o Azure Data Factory?**
    O Azure Data Factory é descrito como um `servico de ingestão de dados`.
    1. Recupera dados de mais de uma fonte de dados e os converte;
    2. Filtra ruidos para manter os dados interessantes;
    3. O trabalho é definido como uma operacaéo de pipeline — é executado continuamente a medida que os dados sao recebidos.

    ![image](https://user-images.githubusercontent.com/86172286/189784223-748f440c-d8a9-43c6-bb9e-36bdbc0b3d32.png)

  - **O que é o Azure Data Lake Storage?**
    O Azure Data Lake Storage é um repositdrio de dados para seu data warehouse moderno.
    1. Organiza os dados em diretorios para acesso aprimorado aos arquivos;
    2. Compativel com permissdes POSIX e RBAC;
    3. Compativel com o Sistema de Arquivos Distribuido Hadoop.

  - **O que é o Azure Databricks?**
    O Azure Databricks é uma plataforma baseada no Apache Spark que oferece processamento e streaming de big data.
    1. Simplifica o provisionamento e a colaboracao de solucdes de analise baseadas no Apache Spark;
    2. Utiliza as capacidades de seguranca do Azure;
    3. Integra-se a uma variedade de servicos de plataforma de dados do Azure e Power BI.
  
  - **O que é o Azure Analysis Services?**
    O Azure Analysis Services cria modelos de tabela para dar suporte a consultas OLAP (processamento analitico online). Ele pode combinar dados de varias fontes, incluindo o Banco de Dados SQL do Azure, o Azure Synapse Analytics, o Azure Data Lake Store, o Azure Cosmos DB e outros.
  
    ![image](https://user-images.githubusercontent.com/86172286/189785054-cff29195-b0fe-4d2f-a051-135ecb8c8e9d.png)

  - **O que é o Azure HDInsight?**
    O Azure HDInsight sao servicos de processamento de big data que permite utilizar bibliotecas pen-source em uma plataforma, em um ambiente Azure.
    
    ![image](https://user-images.githubusercontent.com/86172286/189785182-60e8f9a5-2859-4beb-a9ec-20aca9b2ca0c.png)

### Unidade 1: Verificação de conhecimento

  ![image](https://user-images.githubusercontent.com/86172286/189785810-6b2741ae-2fe4-4382-9e7d-6fada9796d85.png)

  ![image](https://user-images.githubusercontent.com/86172286/189785938-5723b213-6618-4ad0-b9da-667ac12ca489.png)
