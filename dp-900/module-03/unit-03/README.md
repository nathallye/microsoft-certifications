# DP-900: Microsoft Azure Data Fundamentals

## Módulo 3: Explorar os dados não relacionais no Azure

### Unidade 3: Gerenciar armazenamentos de dados não relacionais no Azure

- **Objetivoa da lição 3:**
  1. Carregar dados em um banco de dados Cosmos DB e aprender a consultar esses dados;
  2. Fazer upload e download de dados em uma conta de Armazenamento do Azure.

- **APIs do Cosmos DB:**
  1. **Core(SQL) - Recommended:** Parece muito com um BD SQL, porém separado em containers. Cada container pode ser considerado uma tabela, cada item uma linha. Não necessáriamente esse item tem colunas, ele tem campos/entidades que podemos trabalhar como o NoSQL;
  2. **Azure Cosmos DB API for MongoDB:** Baseado em document;
  3. **Cassandra:** Banco de dados colunar. Recomendado para Big Data e consultas complexas;
  4. **Azure Table:** Parecido com o Storages Table, baseado em chave de partição/Particion Key(chave agrupamento) e uma Chave de Linha/Row Key(chave identificação única). Inclusive podemos começar uma aplicação no Armazenamento de Tabelas/Store Tables no Azure e podemos trocar o SDK para o Cosmos DB e ele continua funcionando igual;
  . **Gremlim:** Graph. Bancos de dados de Gráficos/Graph. Relacionam através de interesses. Recomendado para redes sociais.

  ![image](https://user-images.githubusercontent.com/86172286/189543772-16e5fafb-5f3b-4669-aaf3-bbc5aae34763.png)

- **Demostração de como Configurar a coerência/consistência:**
  Quando usado em apenas uma regiao, o Cosmos DB usa um cluster de servidores. Essa abordagem ajuda a aprimorar a escalabilidade e a disponibilidade. Uma copia de todos os dados é mantida em cada servidor no cluster. 
  
  ![image](https://user-images.githubusercontent.com/86172286/189544253-3a631671-1c7e-4949-a8da-7b8fd15eb460.png)

  Um dos principais diferências do Cosmos DB. Temos algumas opções: 
    1. `Consistência Eventual/Comum` por exemplo, estamos jogando um jogo e uma pessoa do Brasil bateu um record mundial, e primeiro esse record aparece no Brasil(servidor local) e vai replicando essa atualização dos demais servidores das outras regiões conforme as janelas de oportunidade. Mais barato.
    2. `Prefixo Consistênte` ele é muito parecido com o eventual, porém, ele atualiza a informação em todos os servidores de uma vez. Ordena a sequencia dos acontecimento para atualizar. Sequencial. Uniforme.
    3. `Uniforme` por exemplo, temos uma empresa que possui dois serviços, Facebook e Instagram quando publico um story no instagram ele replica automáticamente(na mesma região), no entanto, no facebook essa replicação demora. Acaba entrando no eventual para fazer essas replicações na outra plataforma.
    4. `Desatualizaçã Limitada` ele espera desatualizar em todos, depois ele atualiza todo mundo de uma só vez. Espera todos os bancos de todas as regiões estarem prontos para receber essa nova informação para enviar de uma só vez.
    5. `Forte` é o mais complexo, ele faz e replica para todo mundo de forma assincrona, garante que o dado que está em um está igual para todos os outros. Mais caro.
 
- **Consultas no Azure Cosmos DB:**

  ![image](https://user-images.githubusercontent.com/86172286/189546035-52427cdc-414d-4cbb-b90b-dc199eaaf208.png)
 
  ### Unidade 3: Verificação de conhecimento

  ![image](https://user-images.githubusercontent.com/86172286/189546322-9952e342-aff4-49e0-bd93-e53cdc0d3bb8.png)
