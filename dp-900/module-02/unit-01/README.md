# DP-900: Microsoft Azure Data Fundamentals

## Módulo 2: Explorar os dados relacionais no Azure

- **Objetivos do módulo 1:**
  1. Explorar serviços de dados relacionais no Azure;
  2. Explorar o provisionamento e a implantação de serviços de bancos de dados relacionais no Azure;
  3. Consultar dados relacionais no Azure.

### Unidade 1: Explorar serviços de dados relacionais no Azure

- **Objetivos da unidade 1:**
  - O que são os Serviços de Dados do Azure?
    1. **IaaS vs. Paas**;
    2. **SQL Server em máquinas virtuais do Azure**;
    3. **DB do SQL do Azure**;
    4. **PostgreSQL, MySQL, MariaDB**(opções de Bancos de Dados mais baratas).
    
    ![image](https://user-images.githubusercontent.com/86172286/188325856-8bc1ee54-cf71-4f78-a9cd-05f832e5d24a.png)

- **O que são os Serviços de Dados do Azure?(Para armazenamento relacional)**
  1. **Microsoft SQL Server**;
  2. **MySQL**;
  3. **MariaDB**;
  4. **PostgreSQL**.
  
  ![image](https://user-images.githubusercontent.com/86172286/188325953-04d3ee9c-19e1-4452-8b13-12332e72edb1.png)
  
- **Diferença entre IaaS e PaaS e o Recurso Físico:**
  1. **Físico:** SQL Server local (Máquinas físicas);
  2. **IaaS:** SQL Server no Azure VMs (Máquinas virtuais);
  3. **PaaS:** Banco de Dados SQL do Azure (Bancos de Dados Virtualizados).
  
  - Conclusões:
    1. **Máquinas Físicas:** A longo prazo o `Esforço administrativo` e a `Despesa de capital e controle diário(CAPS)` é muito maior quando temos `bancos de dados locais`(gasto com energia elétrica, licença, máquina, limpeza, atualização, backup);
    2. **IaaS:** Não temos gasto com energia, somente com manutenção, backup;
    3. **PaaS:** Plataforma como serviço, nesse cenário o `Esforço administrativo` e a `Despesa de capital e controle diário(CAPS)` é muito pequeno, pois precisamos ter apenas o esforço de manter os dados, tendo em vista que o backup, licença, atualização, manuntenção é tudo a microsoft que faz.
    
    ![image](https://user-images.githubusercontent.com/86172286/188326191-e1ee2365-45a4-47a6-a747-9983e80018f8.png)

- **Tipos de bancos de dados que temos no Azure:**
  - **SQL Server no Azure:**
    1. **SQL Server em Máquinas Virtuais do Azure:** Opção com menos esforço, por exemplo, no caso de termos um banco de dados local da empresa e queremos levar esse banco de dados para a Nuvem, o que fazemos? Criamos uma máquina virtual e reservamos uma instância da mesma, feito isso, subimos essa máquina para a Nuvem com o banco de dados e a licença. Custo reduzido e Esforço baixo;
    2. **Instância Gerenciada de SQL do Azure:** Já no caso de termos um banco de dados local da empresa e queremos levar esse banco de dados para a Nuvem, mas sem criar uma máquina virtual, desse modo, podemos levar esse banco de dados para uma instância reservada, nesse caso levariamos vários bancos de dados, levariamos o banco e todos os database que esse carinha tem junto;
    3. **Bancos de dados SQL do Azure:** Esse é o modelo `PaaS`, simplesmente usamos.
    
    ![image](https://user-images.githubusercontent.com/86172286/188327153-a32eea78-f9c6-4aea-a132-893e81858d90.png)

- **SQL Server em Máquinas Virtuais do Azure:** 
  É uma solução `IaaS(Infrastructure as a Service/Infraestrutura como Serviço)` que permite que os usuários usem versões completas do SQL Server na nuvem sem precisar gerenciar o hardware local.
    1. Compatibilidade garantia com o SQL Server local;
    2. O cliente gerencia tudo: upgrades de sistema operacional, upgrades de software, backups, replicação;
    3. Pegue pelo servidor e licenças(SQL Server), não por banco de dados.

    ![image](https://user-images.githubusercontent.com/86172286/188328090-1c5d6bb1-b208-43ea-b066-0ac87a2c4642.png) 

- **Bancos de dados SQL do Azure:**
  É uma oferta `PaaS(Platform as a Service/Plataforma como serviço)` onde os usuários criam um servidor de banco de dados gerenciado na nuvem e, em seguida, implementa os bancos de dados no servidor.
    1. Opção de baixo custo com administração mínima;
    2. Melhor para novos projetos na nuvem com design de aplicativo flexível;
    3. Compatível com sistemas de cargas variáveis - faça dimensionamento vertical(significa adicionar mais núcleos de CPU à sua instância de computação.) e horizontal(significa adicionar mais instâncias de computação para sua carga de trabalho. Isso é muito mais econômico e fornece melhor alta disponibilidade do que o dimensionamento vertical) sem reiniciar.
    
    - **Bancos de Dados Individual:** Crie e execute um servidor de banco de dados na nuvem e acesse o banco de dados por meio do servidor;
    - **Pool Elástico:** Vários bancos de dados compartilham os mesmos recursos, como, memória, armazenamento e capacidade de processamento.

    ![image](https://user-images.githubusercontent.com/86172286/188328632-52713c22-aa74-4a5c-9923-22838c13a240.png)

- **Instância Gerenciada de SQL do Azure:**
  Permite que você provisione previamente os recursos computacionais e implemente várias instâncias gerenciadas individuais até seu nível computacional provisionado previamente.
    1. Backups automáticos, correção de software, monitoramento de banco de daos e outras tarefas administrativas;
    2. Quase 100% de compatibilidade com `Microsoft SQL Server` local;
    3. Compatível com outros serviços do Azure;
    4. Conseguimos trabalhar com vários databases por banco de dados.
    
    - **Instância única:** Uma instância do SQL Server, vários bancos de dados;
    - **Pool de instâncias:** Várias instâncias compartilham os mesmos recursos.
    
    ![image](https://user-images.githubusercontent.com/86172286/188329043-f791f0a8-88bd-4284-bcfe-0127d09cd8ea.png)

- **Outro Bancos de Dados que conseguimos trabalhar também:**
  1. **PostgreSQL:** O Banco de Dados do Azure para PostgreSQL é um serviço de banco de dados relacional na nuvem da Microsoft baseado no mecanismo de banco de dados PostgreSQL Community Edition;
  2. **MySQL:** O Banco de Dados do Azure para MySQL é uma implementação PaaS do MySQL na nuvem do Azurew baseada na Community Edition do MySQL;
  3. **MariaDB:** O Banco de Dados do Azure para MariaDB é uma implementação do sistema de gerenciamento de banco de dados MariaDB adaptado para execução no Azure. Baseia-se na Community Edition do MariaDB;

  ![image](https://user-images.githubusercontent.com/86172286/188329377-948908b6-d654-4db8-86ef-b6b181fe2bee.png)

  - **Benefícios do Banco de Dados do Azure para PostgreSQL, MySQL e MariaDB:**
    1. **Banco de dados de comunidade totalmente gerenciado:** Aproveite um serviço totalmente gerenciado e, ao mesmo tempo, use as ferramentas e linguagens que você já conhece;
    2. **Alta disponibilidade integrada para o menor TCO(Total Cost Ownership/Propriedade total de custos):** Garanta que seus dados estejam sempre disponíveis, sem custos adicionais;
    3. **Desempenho e escala inteligentes:** Melhore o desempenho com inteligência integrada e até 16TB de armazenamento e 20 mil IOPs(Input/Output per Second/Operações de entrada e saída por segundo);
    4. **Segurança e conformidade líderes no setor:** Proteja os dados com recursos de segurança avançada, incluindo a Proteção Avançada contra Ameaças;
    5. **Integração com ecossitema do Azure:** Crie aplicativos mais rápidos com os serviços do Azure e preserve a sua inovação com o Azure IP advantage.
  
    ![image](https://user-images.githubusercontent.com/86172286/188329771-bf0f4efa-cf79-48ad-9cad-ebed9f52c558.png)

  
### Unidade 1: Verificação de conhecimento

![image](https://user-images.githubusercontent.com/86172286/188330175-21437484-4b1e-4344-9369-f2981a49e259.png)

![image](https://user-images.githubusercontent.com/86172286/188330333-991779b5-ee05-461b-ac6d-f8e23bfc4b09.png)
