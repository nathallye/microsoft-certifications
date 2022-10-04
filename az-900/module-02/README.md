# AZ-900: Microsoft Azure Fundamentals

## Módulo 2: 

### Principais Serviços do Azure

-  **Regiões**

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
