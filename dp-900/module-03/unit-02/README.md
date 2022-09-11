# DP-900: Microsoft Azure Data Fundamentals

## Módulo 3: Explorar os dados não relacionais no Azure

### Unidade 2

- **Objetivos da unidade 2:**
  a. Provisionar servicos de dados não relacionais;
  b. Configurar servicos de dados nao relacionais;
  c. Explorar os problemas basicos de conectividade;
  d. Explorar os componentes de seguranca de dados.

- **Provisionar servicos de dados não relacionais:**
  - **O que é provisionamento?**
    É a arte de providênciar algo. 
    E o ato de executar uma série de tarefas que um provedor de servicos realiza para criar e configurar um serviço.
    O provisionamento é o processo de definição da infraestrutura de TI. Ele também se refere às etapas necessárias para gerenciar o acesso aos dados e recursos e para disponibilizá-los a usuários e sistemas. 

  - **Como Provisionar o Cosmos DB?**
    O cosmosDB tem 5 APIs diferentes.
      1. Core(SQL)- Recommended;
      2. Azure Cosmos DB API for MongoDB(baseado em document);
      3. Cassandra(banco de dados colunar);
      4. Azure Table(baseado em chave de partição/Particion Key -chave agrupamento- e uma Chave de Linha/Row Key -chave identificação única-);
      5. Gremlim (Graph).
      
      ![image](https://user-images.githubusercontent.com/86172286/189506205-84b0a2e6-aec7-4088-8178-13e0039db1f2.png)

      Para exemplo, vamos usar Core(SQL) para provisionar no Cosmos DB.
      
      1. **Basics:**
      ![image](https://user-images.githubusercontent.com/86172286/189506281-aad4adb4-4043-4820-bdb2-606aee2350da.png)
      
      2. **Global Distribuition:** Só configuramos a `Global Distribuition` quando temos um provisionamento de taxas de transferência(option `Provisioned throughput`.
      
      ![image](https://user-images.githubusercontent.com/86172286/189506286-ac4f3bae-d99b-4ac0-a001-546cc4fa21f1.png)

      3. **Networking:** Vamos deixá-lo disponível para todas as redes(público).
      
      ![image](https://user-images.githubusercontent.com/86172286/189506304-d2143841-6376-42f2-a534-4ca51e658493.png)
      
      4. **Backup Policy:** Temos duas opções - Localmente redundant/`Locally-redundant backup storage` onde esse backup será salvo na mesma região e no mesmo data center; Geograficamente reduntante/`Geo-redundant backup storage` na mesma região em zonas diferentes/data centers diferentes.

      ![image](https://user-images.githubusercontent.com/86172286/189506490-01c71ff8-6103-4dbd-983b-d0ad31f88b05.png)
      
      5. **Encryption:** 
      
      ![image](https://user-images.githubusercontent.com/86172286/189506654-f874d432-4e8e-48ba-a1a3-849d766a73f7.png)

      5. **Tags/Marcações:** Colocar marcações para conseguirmos mapear o custo que isso está nos gerando em cada uma das aplicações ou o BD.

      ![image](https://user-images.githubusercontent.com/86172286/189506701-fe7ddb47-bce2-41ef-845e-58af5f2bc64d.png)
      
      7. **Review + create:**

      ![image](https://user-images.githubusercontent.com/86172286/189506722-0fb54633-fdf0-42f6-a722-284fc9381187.png)

      Seguindo esses passos o nosso recurso está sendo provisionado/preparado/disponibilizado:
      
      ![image](https://user-images.githubusercontent.com/86172286/189506781-dbfc5c95-aa4b-4556-98fb-1890f0654a12.png)

  - **Provisionamento do Data Lake Storage.**

    Primeiro, o que é Data Lake: é um repositório utilizado para armazenar todos os dados estruturados e não estruturados. Ao armazená-los de forma não estruturada pode-se realizar diferentes tipos de análise, incluindo processamento de big data, análise em tempo real e machine learning, a fim de adquirir melhores decisões.
     
    1. **Basics:**
     
    ![image](https://user-images.githubusercontent.com/86172286/189506837-4239b5d3-6d1e-471f-bf82-d26a40928fe4.png)

    2. **Pricing:** 

    ![image](https://user-images.githubusercontent.com/86172286/189506885-fb84d168-7a41-4ae6-9676-c149c2b9e97b.png)

    3. **Encryption:** 
    
    ![image](https://user-images.githubusercontent.com/86172286/189506911-0bc06e80-1943-4e08-b2f6-c6a2600a87f0.png)

    4. **Tags:**

    ![image](https://user-images.githubusercontent.com/86172286/189506941-8ae2e58b-576e-4af8-9072-b5ffae2a0945.png)

    5. **Review + create:**

    ![image](https://user-images.githubusercontent.com/86172286/189506949-52a69304-f1d3-43d6-9d64-60fe8c447f28.png)

    - Também temos a possibilidade de provisionar o Data Lake através do `Storage account`/contas de armazenamento(compartilhamento de arquivos entre usuários de outros serves - podemos ter tabelas, filas e arquivos de compartilhamento). Na janela `Advanced` de criação no tópico `Data Lake Storage Gen2`.
    - `Data Lake Storage Gen2`: Esse cara simplesmente equipara toda a parte de armazenamento de arquivos que temos, ele converte isso como se tivéssemos o preço de armazenamento de larga escala(que geralmente trabalhamos com objetos complexos) e compara isso ao armazenamento tradicional no storage, ou seja, ele não diferencia se estamos usando o storage para guardar um blob ou para guardar um arquivo que vamos trabalhar no Data Lake, com isso temos um alto ganho no custo.

    - Importante: Criar as entidades de segurança. É um objeto que pode ser um usuário, um grupo ou um serviço.

### Unidade 2: Verificação de conhecimento

![Sem título](https://user-images.githubusercontent.com/86172286/189507521-43ecf5d2-453b-42fe-92be-e74b50b62072.png)

