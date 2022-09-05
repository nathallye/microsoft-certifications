# DP-900: Microsoft Azure Data Fundamentals

## Módulo 2: Explorar os dados relacionais no Azure

### Unidade 3: Consultar dados relacionais no Azure

- **Objetivos da unidade 3:**
  1. **Consultar dados relacionais**;
  2. **Descrever as técnicas de consulta de dados usando a linguagem SQL**.

- **Introdução ao SQL:**
  1. O SQL é uma linguagem padrão usada com bancos de dados relacionais;
  2. Os padrões do SQL são mantidos pela ANSI e pela ISO;
  3. Os sistemas RDBMS proprietários têm suas próprias extensões do SQL, como T-SQL, PL/SQL, pgSQL.
  
- **Tipos de instrução SQL:**
  1. **DML(Linguagem de manipulação de dados/Data manipulation language):** Linguagem de manipulação de dados; Usada para `consultar e manipular dados`; SELECT, INSERT, UPDATE, DELETE.
  2. **DDL(Linguagem de definição de dados/Data definition language):** Linguagem de definição de dados; Usada para `definir objetos` de banco de dados; CREATE, ALTER, DROP, RENAME.
  3. **DCL(Linguagem de controle de dados/Data control language):** Linguagem de controle de dados; Usada para gerenciar `permissões` de segurança; GRANT, REVOKE, DENY.

  ![image](https://user-images.githubusercontent.com/86172286/188338487-84a2c83a-f02b-4e13-b55e-c4ac0b465c54.png)

- **Usando instruções DML:**

  ![image](https://user-images.githubusercontent.com/86172286/188338719-dd74601d-dad2-4d67-841f-869abcba0d8d.png)
  
  - **SELECT/SELECIONAR:** Selecionar/ler linhas de uma tabela;
    - **Elementos da instrução SELECT:**
      1. **SELECTED/SELECIONAR (TODOS - *)**;
      2. **FROM/DE**;
      3. **WHERE/ONDE**;
      4. **GROUP BY**;
      5. **ORDER BY**;
      
      Exemplos práticos:
      ``` SQL
      SELECT * # SELECIONAR todos 
        FROM [master].[dbo].[spt_values] # DE DB [master] da tabela dbo os spt_values 
        WHERE number > 1000 # ONDE a coluna number tem valores maior que 1000
        ORDER BY number DESC # ORDENE POR number na ordem decrescente(padrão é ordem crescente - CRES)
      ```
      
      ``` SQL
      SELECT a.type, a.status # SELECIONAR as colunas type e status de a(nomeamos essa tabela assim logo abaixo)
        FROM [master].[dbo].[spt_values] a
        WHERE number > 1000
      ```
      
      ``` SQL
      SELECT a.type, a.status # SELECIONAR as colunas type e status de a(nomeamos essa tabela assim logo abaixo)
        FROM [master].[dbo].[spt_values] a
        WHERE number > 1000
        GROUP BY a.type, a.status # AGRUPAR POR type e status 
      ```
    
  2. **INSERT/INSERIR:** Inserir novas linhas em uma tabela;

    Exemplos práticos:
    ``` SQL
    # A instrução INSERT ... VALUES insere uma nova linha
    
    INSERT INTO [Sales].[OrderDetails]
    (orderid, productid, unitprice, qty, discount)
    VALUES (10255, 39, 18, 2, 0.05);
    ```
    
    ``` SQL
    # Os construtores de tabela e linha adicionam capacidade multilinha à instrução INSERT ... VALUES
    
    INSERT INTO [Sales].[OrderDetails]
      (orderid, productid, unitprice, qty, discount)
    VALUES
      (10256, 39, 18, 2, 0.05),
      (10258, 39, 18, 5, 0.10);
    ```
    
  4. **UPDATE/ATUALIZAR:** Excluir/atualizar linhas existentes em uma tabela;
  5. **DELETE/EXCLUIR:** Excluir linhas existentes em uma tabela.


### Unidade 3: Verificação de conhecimento


