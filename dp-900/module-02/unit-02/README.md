# DP-900: Microsoft Azure Data Fundamentals

## Módulo 2: Explorar os dados relacionais no Azure

### Unidade 2: Explorar o provisionamento e a implantação de serviços de bancos de dados relacionais no Azure

- **Objetivos da unidade 2:**
  1. **Provisionar(providenciar) serviços de dados relacionais**;
  2. **Configurar serviços de dados relacionais**;
  3. **Explorar os problemas básicos de conectividade**;
  4. **Explorar a segurança de dados**.

  ![image](https://user-images.githubusercontent.com/86172286/188333717-83930ec6-07ac-4b7d-9bc0-efdbe7c8f8d8.png)

- **Como configurar serviços de dados relacionais:**

  ![image](https://user-images.githubusercontent.com/86172286/188335635-b0b408ab-cca8-4715-9d07-0d9308c583bd.png)

  1. **Básico/Basics:** Assinatura; Grupo de recursos; Instância Gerenciada/nome do servidor; Nome do Banco de Dados(DB); Logon do Administrador; Senha; Região; Opt-in for pools (DB); Computação + Armazenamento; Tipo de Backup.
  
  - Assinatura/Subscription e Grupo de Recurso/Resource group
 
    ![image](https://user-images.githubusercontent.com/86172286/188334102-ed1dbc51-b35c-4c05-a723-2dcd6f15554b.png)

  - Instância Gerenciada
  
    ![image](https://user-images.githubusercontent.com/86172286/188334134-28f5d78f-88ec-46d8-ad6b-0fa668b07adc.png)

    - Criação do servidor (pois não existe nenhum para selecionarmos) - Nome do Servidor/Server Name e Região/Location

      ![image](https://user-images.githubusercontent.com/86172286/188334232-a7535ce7-66f5-4127-8835-ea2cde4ae6e0.png)

    - Criação do servidor/Create SQL Database Server (pois não existe nenhum para selecionarmos) - Método de Autenticação/Authentication method, Logon do Administrador/Server admin login e Senha/Password
      
      ![image](https://user-images.githubusercontent.com/86172286/188334383-f2c20c11-f36c-4d10-900a-f485cc01155a.png)
    
  -  Selecionar Servidor/Server e Opt-in for pools (DB)
    
    ![image](https://user-images.githubusercontent.com/86172286/188334444-bb9ee5d7-f338-416e-972e-7ef0aee2bbfe.png)

  - Computação + Armazenamento/Compute + storege
    
    ![image](https://user-images.githubusercontent.com/86172286/188334574-663e4817-5f50-4578-bdaf-5a16c1c24c0b.png)

  - Configure database
    - Serverless(Sem servidor)
      
      ![image](https://user-images.githubusercontent.com/86172286/188334619-483e1929-0575-4aa4-9632-b86e08712265.png)
    
  - Tipo de Backup/Backup storage redundancy
    
    ![image](https://user-images.githubusercontent.com/86172286/188334687-e3e69d12-b3ed-4367-a16d-727917b2e3b1.png)
    
  2. **Conectividade de rede/Networking:** Acesso público vs.privado; Regras de firewall/VNet; Tipo de conexão(MI).
    
  - Acesso público vs.privado/Networking connectivity e Regras de firewall/Connection polity
      
    ![image](https://user-images.githubusercontent.com/86172286/188334808-08c70722-f502-4a40-afc1-096ee6139357.png)

  - Tipo de conexão(MI)/Encrypted connections
  
    ![image](https://user-images.githubusercontent.com/86172286/188334844-f41ef976-919e-4500-9205-842881f92a47.png)
  
  3. **Configurações Adicionais:** Fonte de dados(DB). Ordenação do servidor (MI); Ordenação de Banco de Dados(DB); Fuso horário(MI); Aceitar a Segurança de Dados Avançada(DB).
  
   ![image](https://user-images.githubusercontent.com/86172286/188334962-1d0a3c1d-6865-4242-86fd-a82aa18afb1c.png)

   ![image](https://user-images.githubusercontent.com/86172286/188334981-514414f9-a1db-4f0c-b579-e7b34cbde628.png)
  
  4. **Marcas/Tags:**
    
   ![image](https://user-images.githubusercontent.com/86172286/188335026-3b12162b-2f34-4a08-8c12-3d5fdffb4cc8.png)

  5. **Revisão + Criar/Review + create.**
    
- **Conectividade dentro do Azure:**
  `Política de redirecionamento`
  1. Um aplicativo estabelece uma conexão com o banco de dados SQL do Azure através do gateway(gateway refere-se a um pedaço de hardware de rede que possui os seguintes significados: Em uma rede de comunicações, um nó de rede equipado para interfacear com outra rede que usa protocolos diferentes);
  2. Todas as solicitações após a primeira irão diretamente para o banco de dados;
  3. Se a conectividade ao banco de dados falhar, o aplicativo terá que reconectar-se por meio do gateway;
  4. O aplicativo pode ser direcionado a uma cópia diferente do banco de dados executando em outro servidor no cluster(cluster consiste em computadores fracamente ou fortemente ligados que trabalham em conjunto, de modo que, em muitos aspectos, podem ser considerados como um único sistema).

  O ideal é que apontemos o geteway para o cluster e dentro do cluster tem qual é o BD principal.

  ![image](https://user-images.githubusercontent.com/86172286/188335761-dc07b36c-9b8e-499e-b6d3-2e4c72682a14.png)

- **Conectividade de fora do Azure:**
  `Política de Proxy`
  1. Um aplicativo estabelece uma conexão com o banco de dados SQL do Azure por meio do gateway;
  2. Todas as solicitações passam pelo gateway;
  3. O aplicativo pode ser direcionado a uma cópia diferente do banco de dados executando em outro servidor no cluster 

  ![image](https://user-images.githubusercontent.com/86172286/188335895-4f5678ee-e3e1-47f6-8e52-0b6a53f5a365.png)

- **Autenticação e controle de acesso:**

  - **Autenticação forçada em "Modo Misto":**
    Autenticação do SQL/SQL Server authentication e do Azure AD/Azure Active Directory autentication (`Option: Use both SQL and Azure AD authentication`)
      1. Entidade de segurança em nível de servidor para servidor lógico do bano de dados;
      2. Membro da função de servidor sysadmin para MI(Somente sysadmin pode executar inserções em massa para o SQL);

  - **Precisa de autenticação no Windows?(Melhor, mais segura):**
    Use a instânciancia Gerenciada de Autenticação do Azure AD(`Option: Only Azure Active Directory -Azure AD- authentication`)
      1. Administrador de servidor do Azure AD;
      2. Logons do SQL ou do Azure AD;
      3. Usuários de Banco de Dados;
      4. Suportea banco de dados independente do SQL Server.

  - **Banco de Dados SQL do Azure:**
    Autenticação do SQL(`Option: Use SQL authentication`)
      1. Adminstrador de servidor do Azure AD;
      2. Logons do SQL;
      3. Funções loginmanager(gerenciador de login) e dbmanager(o DBManager Professional é uma das mais avançadas ferramentas para gerenciamento de dados) para administradores de servidor limitados;
      4. Usuários de banco de dados;
      5. Usuários de banco de dados contidos(BD contido é um banco de dados isolado de outros bancos de dados e da instância de SQL Server que hospeda o banco de dados), incluindo o Azure AD(recomendado).

  ![image](https://user-images.githubusercontent.com/86172286/188336567-34f66ab5-bab3-4da7-b112-d799fe66c70d.png)

- **RBAC(Controle de Acesso Baseado em Função) do Azure:**
  Ajuda você a gerenciar quem tem acesso aos recursos do Azure e o que é possível fazer com esses recursos.
  Você controla o acesso a recursos usando as atribuições de função. Uma atribuição de função comsiste em três elementos:
    1. **Entidade de segurança:** Um objeto que representa um usuário ou serviço que está solicitando acesso ao recuso do Azure;
    2. **Função:** Uma coleção de permissões;
    3. **Escopo:** Um escopo lista um conjunto de recursos ao qual o acesso se aplica.

  ![image](https://user-images.githubusercontent.com/86172286/188336784-734d03f9-9f1e-445a-8361-d181f680dfd0.png)

- **Banco de Dados do Azure - Réplicas de leitura:**
  As réplicas de leitura `ajudam a melhorar o desempenho e a escala de cargas de trabalho com leitura intensiva`, como Bl e análises. Considere os recursos de réplica de leitura em cenários em que atrasos na sincronização de dados entre o primário e as réplicas são aceitáveis. Crie uma réplica em uma região diferente do Azure com base no primário para um plano de recuperação de desastres em que a réplica substitui o primário em caso de desastres regionais. `O armazenamento de dados nos servidores de réplica aumenta automaticamente sem afetar as cargas de trabalho`.
  
  ![image](https://user-images.githubusercontent.com/86172286/188336962-47f3abac-c26f-472a-905a-3106010c568e.png)

