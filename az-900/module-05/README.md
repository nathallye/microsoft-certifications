# AZ-900: Microsoft Azure Fundamentals

## Módulo 5: Identidade, governança, privacidade e conformidade

### Principais servicos de identidade do Azure

- **Servicos de identidade do Azure - Domínio de objetivo**

- Explicar a diferença entre autenticação e autorização;
- Definir o Azure Active Directory;
- Descrever a funcionalidade e o uso do Azure Active Directory;
- Descrever a funcionalidade e uso do Acesso Condicional, Autenticação Multifator (MFA) e Logon Unico (SSO).

- **Comparar autenticação e autorização**

`Autenticação`
  - Identifica a pessoa ou serviço buscando acesso a um recurso.
  - Solicita credenciais de acesso legítimo.
  - Base para criar principios de identidade e controle de acesso seguros.

`Autorização`
  - Determina o nivel de acesso de uma pessoa ou serviço autenticado.
  - Define quais dados eles podem acessar e o que podem fazer com eles.

Autenticação é quando você pode acesssar. E até onde você pode ir é sua Autorização.

![image](https://user-images.githubusercontent.com/86172286/194387416-69e0ccb3-7bd2-4d01-ba87-fd3758fcf5df.png)

**Autenticacao multifator do Azure**

Fornece segurança adicional para as identidades, exigindo dois ou mais elementos para autenticação completa.
Algo que você sabe <--> Algo que você tem <--> Algo que vocé é

![image](https://user-images.githubusercontent.com/86172286/194387473-4118f3b1-b25e-4203-8fb7-72b276b93ffe.png)

- **Azure Active Directory (AAD):**

O Azure Active Directory (AAD) é 0 servico de gerenciamento de acesso e identidade baseado em nuvem do Microsoft Azure.

- Autenticacão (credenciais dos funcionários para acessar os recursos).
- Logon unico (SSO)
- Gerenciamento de aplicativos.
- Entre empresas (B2B) - Federação relação de segurança
- Serviços de identidade entre empresa e cliente (B2C).
- Gerenciamento de dispositivos.

Gerenciador de domínio e válidação usuário e senha.

**Acesso condicional**

Politica aplicada para cada usuário ou grupo de usuários.

![image](https://user-images.githubusercontent.com/86172286/194389037-8f73ec4f-68e7-44b0-8316-b6d4ab69d25e.png)

### Governança

- **Metodologias de governança do Azure - Domínio de objetivo**

Descrever a funcionalidade e o uso de:

  - RBAC (controle de acesso baseado em função) 
  - Bloqueios de recursos
  - Marcas
  - Azure Policy
  - Azure Blueprints
  - Cloud Adoption Framework para o Azure

- **Explorar RBAC (controle de acesso baseado em função)**

  - Gerenciamento de acesso de granularidade fina.
  - Divida as tarefas dentro da equipe e conceda somente a quantidade de acesso de que os usuários precisam para trabalhar.
  - Habilite o acesso ao portal do Azure e o controle de acesso aos recursos.

![image](https://user-images.githubusercontent.com/86172286/194427213-7bb4991d-9173-4445-9db4-aa68caca5e34.png)

- **Bloqueios de recursos**

1. Proteja os recursos do Azure de exclusão ou modificacão acidental.
2. Gerencie bloqueios nos níveis de assinatura, grupo de recursos ou recursos individuais no portal do Azure.

![image](https://user-images.githubusercontent.com/86172286/194427330-0c715e37-6966-4c8f-90a4-826ccce77cf9.png)

- **Marcas/Tags**

1. Fornecem metadados aos recursos do Azure.
2. Organizam os recursos em uma taxonomia de maneira lógica.
3. Consistem em um par nome-valor.
4. Muito úteis para reunir informacões de cobrança.

![image](https://user-images.githubusercontent.com/86172286/194428527-c50e5d7a-f904-483a-b4ce-5e27a695b15d.png)


- **Azure Policy**

O Azure Policy ajuda a impor padrões organizacionais e avaliar conformidade em escala. Fornece governança e consistência de recursos com conformidade regulamentar, segurança, custos e gerenciamento.

- Avalia e identifica os recursos do Azure que não atendem as suas politicas.
- Fornece definições de politicas e iniciativas integradas, em categorias como Armazenamento, Rede, Computação, Central de Segurança e Monitoramento.

Gestão das regras do negocio.

- **Azure Blueprints**

O Azure Blueprints possibilita que as equipes de desenvolvimento criem e implantem novos ambientes com rapidez. As equipes de desenvolvimento podem desenvolver a confiança rapidamente por meio de conformidade organizacional com um conjunto de componentes integrados (como rede) para acelerar o desenvolvimento e a entrega.

- Atribuições de função
- Atribuicões de politica
- Modelos do Azure Resource Manager
- Grupos de recursos

- **Cloud Adoption Framework**

- A abordagem One Microsoft para adocão de nuvem no Azure.
- Melhores práticas dos funcionários, parceiros e clientes da Microsoft.
- Ferramentas, orientações e narrativas para estratégias e resultados.
