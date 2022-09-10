# DP-900: Microsoft Azure Data Fundamentals

## Módulo 3: Explorar os dados não relacionais no Azure

- **Objetivos módulo 1:**
  1. Explorar serviços de dados não relacionais no Azure;
  2. Explorar o provisionamento e a implantação de serviços de dados não relacionais no Azure;
  3. Gerenciar armazenamento de dados não relacionais no Azure.

### Unidade 1: Explorar serviços de dados não relacionais no Azure;

- **Objetivos da unidade 1:**
  1. Explorar os casos de uso e os benefícios de gerenciamento do uso do Armazenamento de Tabelas no Azure;
  2. Explorar os casos de uso e os benefícios de gerenciamento do uso do Armazenamento de Blobs do Azure;
  3. Explorar os casos de uso e os benefícios de gerenciamento do uso do Armazenamento de Arquivos do Azure;
  4. Explorar os casos de uso e os benefícios de gerenciamento do uso do Azure CosmosDB.
  
- **Explorar os casos de uso e os benefícios de gerenciamento do uso do Armazenamento de Tabelas/Store Tables no Azure:**
  Temmos uma Chave de Partição/`Particion Key(Chave agrupamento)` e uma Chave de Linha/`Row Key(chave identificação única)`.
  Ex.: Digamos que, dentro da cidade de SP temos uma Particion Key chamada Cidade e uma Row Key que é o titulo de eleitor e nessa chave de linha teremos todas as informações do eleitor de determinada cidade(grupo).
  
  ![image](https://user-images.githubusercontent.com/86172286/189469127-012d9ff2-f9ca-4fad-98e7-1bef14ca9ec5.png)
  
  ![image](https://user-images.githubusercontent.com/86172286/189468522-8174dce1-abb4-470f-b5b3-487f73d74261.png)

- **Explorar os casos de uso e os benefícios de gerenciamento do uso do Armazenamento de Blobs do Azure(opção disponível apenas na conta premium/premium account):**

  - **Blobs de blocos:** (ex.: backups, arquivos de carga de dados)
    a. Seu `tamanho máximo é de 4,7TB`;
    b. Ideais para armazenar objetos `binários grandes e discretos que mudam com pouca frequência`;
    c. Cada bloco pode armazenar até `100MB de dados`;
    d. Um blob de bloco pode conter `até 50 mil blocos`.
    
    ![image](https://user-images.githubusercontent.com/86172286/189469290-a86459d9-9cd5-4cf0-8fd9-ab3d1aa78bab.png)
    
    No memento que criamos um blob e não especificamos o tipo por padrão será um blob de bloco. 
  
  - **Blobs de páginas:** (ex.: disco de Máquina Virtual)
    a. Podem armazenar até `8TB` de dados;
    b. São organizados como uma `coleção de páginas de tamanho fixo de 512 bytes`;
    c. Usados para implementar o armazenamento em disco virtual para máquinas virtuais;
  
  - **Blobs de acréscimo:**
    a. Seu tamanho maximo é de mais de `195GB`;
    b. E um blob de blocos `usado para otimizar operacões de acréscimo`;
    c. Cada bloco pode armazenar `até 4MB` de dados.
    
  ![image](https://user-images.githubusercontent.com/86172286/189468719-6198a9e2-6752-4732-94e9-2afe58b278db.png)
 
- **Explorar os casos de uso e os benefícios de gerenciamento do uso do Armazenamento de Arquivos do Azure("file share"):**
  Cria compartilhamentos de arquivo na nuvem e oferece a capacidade de acessar esses compartilhamentos de qualquer lugar com uma conexão à internet;
  
  ![image](https://user-images.githubusercontent.com/86172286/189469173-2f37222f-d60e-411b-bfb2-cce79a8531fb.png)
  
  a. Usa o Server Message Block 3.0 (SMB) para compartilhar arquivos;
  b. Compartilhe até 100 TB de dados em uma conta de armazenamento;
  c. Servico totalmente gerenciado - os dados sao replicados localmente e é criptografado em REST.
  
  ![image](https://user-images.githubusercontent.com/86172286/189469060-79b869f8-0a9a-48c2-a094-db1b660daf77.png)

  
### Unidade 1: Verificação de conhecimento

