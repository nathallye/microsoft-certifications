# AZ-900: Microsoft Azure Fundamentals

## Módulo 4: Segurança

### Recursos de Segurança do Azure

- **Central de Segurança do Azure/Microsoft Defender for Cloud**

A Central de Segurança do Azure é um serviço de monitoramento que fornece proteção contra ameacas nos datacenters do Azure e nos datacenters locais.

  - Fornece recomendações de segurança
  - Detectar e bloquear malwares
  - Analisar e identificar possiveis ataques
  - Controle de acesso just-in-time para portas
  
  ![image](https://user-images.githubusercontent.com/86172286/194377866-30f37cf7-dd1d-497c-b506-98b7f11a7ada.png)

- **Azure Sentinel**

O Azure Sentinel é uma solução de gerenciamento de informações de segurança (SIEM) e de resposta automatizada de segurança(SOAR) que fornece uma análise de segurança e inteligência contra ameaçaas em uma empresa.

Conector e Integrações:

  - Office 365
  - Azure Active Director
  - Proteção Avançada contra
  - Ameaças do Azure
  - Microsoft Cloud App Security

![image](https://user-images.githubusercontent.com/86172286/194377955-e1981c40-5b5a-4a83-a9b0-7f680371b578.png)

- **Azure Key Vault**

O Azure Key Vault armazena segredos do aplicativo em um local de nuvem centralizado para controlar com segurança as permissões e o registro em log de acesso.

  - Gerenciamento de segredos.
  - Gerenciamento de chaves.
  - Gerenciamento de certificados.
  - Armazenar segredos apoiados por módulos de segurança de hardware (HSMs).

- **Host Dedicado do Azure**

O Host Dedicado do Azure fornece servidores físicos que hospedam uma ou mais máquinas virtuais do Azure dedicadas a carga de trabalho de uma única organização.

Beneficios
  - Isolamento do hardware no nivel do servidor
  - Controle sobre o tempo do evento de manutenção
  - linhado com os Beneficios Hibridos de Uso do Azure

### Conectividade de rede segura

- **Protecgado completa/Sistemas de Camadas**

1. Uma abordagem em camadas para proteger sistemas de computador.
2. Fornece vários níveis de proteção.
3. Ataques contra uma camada são isolados das camadas subsequentes.

Camadas:
  - Segurança física
  - Identidade e acesso
  - Perímetro
  - Rede
  - Computação
  - Aplicativo
  - Dados

- **Seguranca Compartilhada**

- Migrar de datacenters controlados pelo cliente para datacenters baseados em nuvem muda a responsabilidade pela segurança.
- A segurança se torna um interesse compartilhado entre provedores de nuvem e clientes.

Ficar atento no que é minha responsabilidade como cliente e o que é responsabilidade do provedor(microsoft) a depender do sistema.

![image](https://user-images.githubusercontent.com/86172286/194381784-b593793a-8ac4-4984-890a-6404a8aafde1.png)


- **Grupos de Segurança de Rede (NSGs)/ Network Security Group**

Os Grupos de Segurança de Rede (NSGs) filtram o tráfego de rede para os recursos do Azure (e a partir dele também) nas Redes Virtuais do Azure.

  1. Definir regras de entrada e de saída para filtrar por fonte e endereço IP de destino porta e protocolo.
  2. Adicionar várias regras, conforme necessário, dentro dos limites da assinatura.
  3. O Azure aplica regras de segurança de linha de base, padrão aos novos NSGs.
  4. Substituir as regras padrão por reagras novas e de prioridade mais alta. 

- **Firewall do Azure**

Um Firewall como Serviço (FaaS) com estado e gerenciado que concede/nega acesso ao servidor com base no endereco IP de origem, para proteger recursos de rede.

  1. Aplica regras de filtragem de trafego de entrada e de saída
  2. Alta disponibilidade integrada
  3. Escalabilidade de nuvem irrestrita
  4. Usa registro em log do Azure Monitor

O `Gateway` de Aplicativo do Azure também fornece um firewall, chamado de Firewall de Aplicativo Web (WAF). O WAF fornece protecao interna, centralizada para seus aplicativos Web.

`Network Security Group` protege o uso interno da assinatura o `Firewall` protege dos acessos externos e protege o próprio usuário de sair pra fora(trafego externo).

- **Proteção contra DDoS (Negação de Serviço Distribuida) do Azure**

Os ataques DDoS sobrecarregam e esgotam recursos de rede, tornando os aplicativos lentos ou não responsivos.

  1. Limpa o trafego de rede indesejado antes que ele afete a disponibilidade do serviço.
  2. A camada de serviço básica é automaticamente ativada no Azure.
  3. A camada de serviço padrão adiciona recursos de mitigacão ajustados para proteger os recursos de Rede Virtual do Azure.