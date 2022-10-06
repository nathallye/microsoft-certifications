# AZ-900: Microsoft Azure Fundamentals

## Módulo 2: Principais Serviços do Azure

### Regiões

O Azure oferece mais regiões globais do que qualquer outro provedor de nuvem com mais de 60 regides representando mais de 140 paises.

  1. As regiões são compostas de um ou mais datacenters muito próximos. 
  2. Fornecer flexibilidade e escala para reduzir a latência do cliente.
  3. Preservar a residência de dados com uma oferta de conformidade abrangente.
  
  ![image](https://user-images.githubusercontent.com/86172286/193947664-038ebe04-da4e-40e5-bb3a-41863ae31707.png)

-  **Pares de Regiões**

  1. No minimo 300 milhas de separação entre pares de regiões.
  2. Replicações automática para alguns serviços.
  3. Recuperação de região priorizada em caso de interrupção.
  4. As atualizações são lançadas sequencialmente para minimizar o tempo de inatividade.

  ![image](https://user-images.githubusercontent.com/86172286/193947700-c9ff679c-ddbe-48b5-89c1-c2fd2d55ff73.png)
  
- **Opções de Disponibilidade**

![image](https://user-images.githubusercontent.com/86172286/193947997-5fdb4c3c-067e-47f8-b85e-ae0b4ced6226.png)

- **Zonas de disponibilidade**

  1. Oferecer proteção contra tempo de inatividade por causa de falha do datacenter.
  2. Separar fisicamente os datacenters dentro da mesma região.
  3. Cada datacenter é equipado com alimentação, resfriamento e rede independentes.
  4. Conectado por meio de redes privadas de fibra óptica.

  Cada Região do Azure, possui zonas de disponibilidade e podemos navegar entre essas zonas caso uma venha a falhar.
  
  ![image](https://user-images.githubusercontent.com/86172286/193948293-254ffe81-98bb-4a85-a21a-89b77758e3fb.png)

### Recursos do Azure

Recursos do Azure são componentes como armazenamento, máquinas virtuais e redes que estado disponíveis para criar soluções em nuvem.

  1. Máquinas Virtuais
  2. Contas de Armazenamento
  3. Redes Virtuais
  4. Serviços de Aplicativos
  5. Bancos de Dados SQL
  6. Funções

São itens que colocamos, ou criamos, ou provisionamos dentro dos serviços do Azure.

![image](https://user-images.githubusercontent.com/86172286/193949646-177fe92a-c977-4c00-a362-00ab9c922ce4.png)

- **Grupos de recursos**

Um grupo de recursos é um contêiner para gerenciar e agregar recursos em uma única unidade.
  1. Os recursos podem existir em apenas um grupo de recursos.
  2. Os recursos podem existir em diferentes regiões.
  3. Os recursos podem ser movidos para diferentes grupos de recursos.
  4. Os aplicativos podem utilizar vários grupos de recursos.

Um recurso precisa de um grupo de recurso criado. É um agrupamento lógico. Não é físico, é virtual. É um contêiner.

![image](https://user-images.githubusercontent.com/86172286/193949768-024db2a5-0ef8-4718-9227-01c09bfb5785.png)

- **Azure Resource Manager**

O Azure Resource Manager(ARM) oferece uma `camada de gerenciamento` que permite que você crie, atualize e exclua recursos na sua assinatura do Azure.
Principal vantagem, gerênciamento de infraestrutura e gerênciamento de permisionamento(conseguimos gerar o recurso com as permissões dividamente criadas e liberadas).

![image](https://user-images.githubusercontent.com/86172286/193950275-f4078ce2-48e7-46c9-a4b8-509e2658a50a.png)

- **Assinaturas do Azure**

Uma assinatura do Azure fornece a você acesso autenticado e autorizado às contas do Azure.

  1. `Limite de cobrança`: gerar faturas e relatórios de cobrançaa separados para cada assinatura.
  2. `Limite de controle de acesso`: gerenciar e controlar o acesso aos recursos que os usuários provisionam com assinaturas especificas.

![image](https://user-images.githubusercontent.com/86172286/193950299-13d3cd9e-756d-4420-ac9e-3f0b2c31ed27.png)

- **Grupos de Gerenciamento**

1. Os grupos de gerenciamento podem incluir várias assinaturas do Azure.
2. As assinaturas herdam as condições aplicadas ao grupo de gerenciamento.
3. E possivel oferecer suporte a 10.000 grupos de gerenciamento em um único diretório.
4. Uma arvore de grupos de gerenciamento pode oferecer suporte a até seis níveis de profundidade.

Estrutura de árvore/hierarquia onde aplicamos as condições de gerênciamento e tudo isso reflete nas assinaturas abaixo.

![image](https://user-images.githubusercontent.com/86172286/193950827-f5213ef1-4d87-4aea-9616-6e68c476ac06.png)

- **Serviços de computação do Azure**

A computação do Azure é um serviço de computação sob demanda que fornece recursos de computação, como discos, processadores, memória, rede e sistemas operacionais.

  1. `Máquinas Virtuais`
  As Máquinas Virtuais (VM) do Azure são emulacões de software de computadores físicos.
    - Inclui processador virtual, memória armazenamento e rede.
    - Oferta de IaaS que oferece personalização e controle total.

  2. `Serviço de Aplicativo do Azure`
  O Serviço de Aplicativo do Azure é uma plataforma totalmente gerenciada para criar, implantar e escalar aplicativos Web e APIs com rapidez.
    - Trabalha com .NET, .NET Core, Node,js, Java, Python ou php.
    - Oferta de PaaS com requisitos de nível corporativo de desempenho, segurança e conformidade.

  3. `Instâncias de Contêiner do Azure`
  Os Contêineres do Azure sdo um ambiente virtualizado leve que não exige gerenciamento do sistema operacional e pode responder a mudanças sob demanda.
    - `Instâncias de Contêiner do Azure:` uma oferta do PaaS que executa um contêiner no Azure sem precisar gerenciar uma máquina virtual ou serviços adicionais.
    - `Serviço de Kubernetes do Azure:` um serviço de orquestração para contêineres com arquiteturas distribuidas e grandes volumes de contêineres.

  4. `Área de Trabalho Virtual do Azure`
  A Área de Trabalho Virtual do Azure é uma virtualização de desktop e aplicativo que roda na nuvem.
    - Criar um ambiente completo de virtualização da área de trabalho sem precisar executar outros servidores de gateway. 
    - Publicar pools de host ilimitados para acomodar várias cargas de trabalho.
    - Reduzir custos com recursos em pool, com várias sessões.

- **Serviços de rede do Azure**

A `Rede Virtual (VNet) do Azure` permite que recursos do Azure se comuniquem entre si, com a Internet e com redes locais.

O `Gateway de Rede Virtual Privada (VPN)` é usado para enviar tráfego criptografado entre uma rede virtual do Azure e um local na Internet pública.

O `Express Route do Azure` amplia redes locais para o Azure por meio de uma conexao privada facilitada por um provedor de conectividade.

- **Serviços de armazenamento do Azure**

O `armazenamento de contêiner (blob)` é otimizado para armazenar grandes quantidades de dados não estruturados, como dados binários ou de texto.

O` armazenamento em disco` fornece discos para máquinas virtuais, aplicativos e outros serviços acessarem e usarem.

Os `Arquivos do Azure` configuram compartilhamentos de arquivos de rede altamente disponíveis que podem ser acessados usando o protocolo padrão Bloco de Mensagens do Servidor (SMB).

### Serviços de Banco de Dados do Azure

O `Azure Cosmos Database` é um serviço de banco de dados distribuido globalmente que escala de maneira elástica e independente a taxa de transferência e o armazenamento.

O `Banco de Dados SQL do Azure` é um banco de dados relacional como serviço (DaaS) baseado na última versão estável do mecanismo de banco de dados do Microsoft SQL server.

O `Banco de Dados do Azure para MySQL` é um serviço do banco de dados MySQL totalmente gerenciado para desenvolvedores de aplicativos.

O `Banco de Dados do Azure para PostgreSQL` é um serviço de banco de dados relacional baseado no mecanismo de banco de dados Postgres open-source.

- **Instância Gerenciada de SQL do Azure**

A Instância Gerenciada de SQL do Azure permite que os clientes existentes do SQL Server fagam “lift and shift” dos aplicativos locais para a nuvem com o mínimo de alteracdes no aplicativo e no banco de dados.

  - Plataforma como serviço totalmente gerenciada e sempre atualizada.
  - Preserva todos os recursos do `PaaS` (atualizações de versão e aplicacado de patch automáticas, backups automatizados e alta disponibilidade)
  - Troca as licenças existentes para taxas descontadas na instância Gerenciada de SQL usando 0 Beneficio Hibrido do Azure.

### Explorar o Azure Marketplace

O Azure Marketplace permite que os clientes localizem, experimentem, comprem e provisionem aplicativos e serviços de centenas dos principais provedores de serviço,
todos certificados para execução no Azure.

  - Plataformas de contêiner open-source.
  - Imagens da máquina virtual e do banco de dados.
  - Software de compilação e implantação de aplicativos.
  - Ferramentas para desenvolvedores.
  - E muito mais, com mais de 10.000 itens listados!
  
- **Camadas de acesso de armazenamento do Azure**

![image](https://user-images.githubusercontent.com/86172286/194191736-f29532f7-554a-4994-aaf9-722e6217cdbf.png)
