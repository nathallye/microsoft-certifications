# DP-900: Microsoft Azure Data Fundamentals

## Módulo 1: Explorar os principais conceitos de dados

### Unidade 3: Descrever os conceitos de dados relacionais

- **Identificar casos de uso de banco de dados relacionais:**

  1. **IoT:** Embora sejam normalmente considerados como não relacionais, os dados de dispositivos IoT poderiam ser estruturados e consistentes;
  2. **Processamento de transação on-line:** Por exemplo, sistemas de pedodps qie realizam muitas atualizações transacionais pequenas;
  3. **Data warehousing:** Grandes quantidade s de dados podem ser importadas de várias fontes e estruturadas para permitir consultas de alto desempenho.
  
![image](https://user-images.githubusercontent.com/86172286/188292585-dddab79e-c19e-4f69-b373-8baa5b076021.png)

- **Como funciona um BD relacional/SQL?**
  1. Os dados são armazenados em uma tabela;
  2. A tabela consiste em linhas e colunas;
  3. Todas as linhas têm o mesmo número de colunas;
  4. Cada coluna é definida  por um tipo de dados.

![image](https://user-images.githubusercontent.com/86172286/188292623-15101420-e01d-475d-95eb-07826f97be93.png)

- **Entidades:**
Uma entidade é uma representação de um item que pode ser físico(como um cliente ou produto), o virtual(como um pedido). As entidades são conectadas por relações que permitem a interação. Por exemplo, um cliente pode fazer um pedido de um produto.

- **Normalização(3NF - 3° Forma Normal):**
  1. Reduzir armazenamento;
  2. Evitar a duplicação de dados;
  3. Melhorar a qualidade dos dados.
  
![image](https://user-images.githubusercontent.com/86172286/188292776-c8eef0e4-8cf8-4346-a8bc-61b9d52e6b4a.png)

- **Relações:**
  1. As chaves primárias e estrangeiras são usadas para definir relacionamentos;
  2. Não há nenhuma duplicação de dados (a não ser valores chave);
  3. Os dados são recuperados unindo as tabelas em uma consulta.
  
![image](https://user-images.githubusercontent.com/86172286/188292853-907522df-849e-4857-bdee-752f109b5d92.png)

- ** Tipos de Índices:**
  1. Clusterizado: Um índice clusterizado determina a ordem em que as linhas de uma tabela são armazenadas no disco. Se uma tabela tem um índice clusterizado, no momento de um INSERT as linhas dessa tabela serão armazenadas em disco na ordem exata do mesmo índice.

  2. Não-clusterizados: Já os índices não-clusterizados não fazem esse trabalho de ordenação dos dados tal qual é feito com os índices clusterizados. Em outras palavras, enquanto os índices clusterizados ordenam fisicamente tanto as linhas da tabela quanto os próprios índices e mantêm os mesmos próximos uns aos outros; os não-clusterizados ordenam somente o índice em si, e não as linhas (que são salvas sempre de forma aleatória no disco).
  Numa tabela, quando é definida uma chave primária, um índice clusterizado é criado automaticamente pelo banco para a mesma. E o que ele faz basicamente é ordenar as informações pela coluna de chave daquele índice em disco.

- **Vantagems dos Índices:**
  1. Otimiza consultas de pesquisa para recuperação mais rápida de dados;
  2. Reduz a quantidade de páginas de dados que precisam ser lidas para recuperar os dados em uma declaração SQL;
  3. Os dados são recuperados unindo as tabelas em uma consulta.

- **Exibição/Views:**
Uma exibição/view é uma tabela virtual com base no conjunto de resultados de uma consulta.
  1. As exibições são criadas para simplificar a consulta;
  2. Combine dados relacionais em uma exibição de painel simples.

### Unidade 3: Verificação de conhecimento

![image](https://user-images.githubusercontent.com/86172286/188293121-d8d69d2b-08ab-4eeb-b5b1-ed695901f45a.png)
