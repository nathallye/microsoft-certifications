# DP-900: Microsoft Azure Data Fundamentals

## Módulo 1: Explorar os principais conceitos de dados

### Unidade 4: Explorar os conceitos dos dados não relacionais

CosmosDB
StoreTable

- **Identificar casos de uso o banco de dados não relacional/NoSQL:**
  1. **IoT e telemática:** Com frequência exigem ingerir grandes quantidades de dados em frequentes explosões de atividades, os dados são semiestruturados ou estruturados, com frequência exigem processamento em tempo real;
  2. **Varejo e marketing:** Cenários comuns para dados distribuídos globalmente, armazenamento de documentos;
  3. **Jogos:** Estatísticas de jogo, integração com mídias sociais, quadros de líderes, aplicativos de baixa latência;
  4. **Web e móvel:** Normalmente usado com análises de cliques na web, aplicativos modernos incluindo bots.

![image](https://user-images.githubusercontent.com/86172286/188293688-163658f3-399b-4399-9255-99036a5821a2.png)

- **Entidades:**
Coleções não relacionais podem ter...
  1. Várias entidades na mesma coleção ou contêiner com diferentes campos;
  2. Têm um esquema diferente, não tabular;
  3. São frequentemente definidos por identificar cada campo com o nome que ele representa;
  4. Flexível para dados não conhecidos.

![image](https://user-images.githubusercontent.com/86172286/188293388-1f3d9fe6-0f49-4d2f-a02f-c9344a5b0f76.png)

- **Tipos de dados usados em BD's não relacionas:**
  - Dados semiestruturados:
    A estrutura de dadps é definida dentro dos dados reais por campos. O formato/tipos de arquivos incluem:
      1. **JSON:** Chaveado, delimita e XML;
![image](https://user-images.githubusercontent.com/86172286/188293769-c98dcc26-697b-4caf-b5ac-b1849ac16192.png)
      2. **AVRO:** Criado pelo Apache, cada registro tem a informação do campo e o tipo;
![image](https://user-images.githubusercontent.com/86172286/188293799-1874d336-0b02-4a7f-bbb5-3683646fe85e.png)
      3. **ORC - Optimized Row Columnar:** Modelo colunar de banco de dados;
![image](https://user-images.githubusercontent.com/86172286/188293847-1e28cc80-0785-4653-88e0-26acbfac9d0b.png)
      4. **Parquet:** Formato de arquivo gratuito e de código abertp; Formato baseado em coluna; Usado para casos de uso de análise (OLAP), normalmente em conjunto com BD's OLTP tradicionais; Compressão e descompressão de dados altamente eficientes; Suporta tipos de dados complexos e estruturas de dados aninhadas avançadas.
      
- **O que é NoSQL?**

![image](https://user-images.githubusercontent.com/86172286/188293975-e8a4ac30-2736-4501-8bee-aa22fc25ad8d.png)

  1. Respositórios de chave-valor;
  2. Baseados em documento; Ex.: MongoDB - O Cosmos DB consegue trabalhar com a API do Mongo
  3. Bancos de dados de família de colunas;
  4. Bancos de dados de grafo/gráficos.
  ![image](https://user-images.githubusercontent.com/86172286/188293987-ab55595a-fe4f-4e9f-9cff-65e5af5e37ec.png)

### Unidade 4: Verificação de conhecimento

![image](https://user-images.githubusercontent.com/86172286/188294069-9f6ada34-fc79-47f2-bee5-0e8bfe0d452c.png)
