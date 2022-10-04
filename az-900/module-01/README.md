# AZ-900: Microsoft Azure Fundamentals

## Módulo 1: Conceitos em Nuvem

### O que é computação em Nuvem?

- Computação em Nuvem é a entrega de servicos de computação por meio da Internet, possibilitando uma inovação mais rapida, recursos flexiveis e economia de escala.

- Computação em Nuvem não é só cumpatação é trazer um serviço para a nuvem. Usar o poder de processamento da nuvem, poder de armazenamento, poder de análise, para seu modelo de trabalho.
  
  1. Computação;
  2. Rede;
  3. Armazenamento;
  4. Análise.
  
  ![image](https://user-images.githubusercontent.com/86172286/193884554-f0795cb0-b998-4986-9c3b-9470b025ce8e.png)

### Modelos de Nuvem

- **Nuvem pública**

  1. Pertencente a servicos de nuvem ou provedor de hosting.
  2. Fornece recursos e serviços a várias organizações e usuários.
  3. Acessado via conexão de rede segura (geralmente pela Internet).

  Ex.: AWS, AZURE, GCP,...

  Conseguimos provisionar serviços de formas simples e rápida, e com o custo controlado.

  ![image](https://user-images.githubusercontent.com/86172286/193884605-426f3c54-2632-4d49-8eb3-a005aba02bc3.png)

- **Nuvem privada**

  1. As organizações criam um ambiente em nuvem em seu datacenter.
  2. A organização é responsável por operar os serviços que fornece.
  3. Não fornece acesso aos usuários fora da organização.

  Ex.: Datacenter da empresa.
  
  ![image](https://user-images.githubusercontent.com/86172286/193886043-c4a11bad-e9a4-4021-8d7c-b71febed0158.png)

- **Nuvem híbrida**

  1. Combina as nuvens `Pública` e `Privada` para permitir que os aplicativos sejam executados no local mais apropriado.

  Conseguimos expandir o poder computacional de uma nuvem privada com a nuvem pública, tornando o modelo híbrido.

  ![image](https://user-images.githubusercontent.com/86172286/193886141-1a07399d-2cde-4070-9c3a-0eeb071be7de.png)


- **Comparação dos modelos de nuvem**

  - `Nuvem publica`
    1. Nenhuma despesa de capital para escalar verticalmente.
    2. Os aplicativos podem ser rapidamente provisionados e desprovisionados.
    3. As organizacées pagam apenas pelo que usam.
    
  - `Nuvem privada`
    1. O hardware deve ser adquirido para inicialização e manutenção.
    2. As organizações têm controle total sobre recursos e segurança.
    3. As organizações são responsáveis pelas atualizações e pela manuteção do hardware.

  - `Nuvem Hibrida`
    1. Oferece a maior flexibilidade.
    2. As organizações determinam onde executar seus aplicativos.
    3. As organizações controlam os requisitos de segurança, conformidade ou jurídicos.

  ![image](https://user-images.githubusercontent.com/86172286/193887476-a459b9c3-90cf-4e6b-88eb-1b3d0b9fa17f.png)
  
### Considerações e benefícios da Nuvem

- **Benefícios da Nuvem**

  1. Alta disponibilidade; SLA - Tempo de disponibidade do serviço.
  2. Escalabilidade;
  3. Alcance global;
  4. Agilidade;
  5. Recuperação de desastre;
  6. Tolerancia a falhas;
  7. Elasticidade;
  8. Capacidade de latência do cliente;
  9. Considerações sobre custo preditivo;
  10. Segurança.

  ![image](https://user-images.githubusercontent.com/86172286/193890083-7c22bbd3-d989-4224-9441-e1cfd24f6155.png)

- **Comparar CapEx e OpEx**

  - `Despesas de Capital (CapEx)`
    1. O gasto inicial de dinheiro na infraestrutura física.
    2. Os custos de CapEx têm um valor que é reduzido ao longo do tempo.

  - `Despesas Operacionais (OpEx)` - Cloud é tudo OpEx
    1. Gastos em produtos e serviços conforme necessário, pagamento conforme o uso.
    2. Receber a conta imediatamente.

  ![image](https://user-images.githubusercontent.com/86172286/193890143-58a86f2e-a6de-4559-82bc-f862a960f47a.png)

### Serviços de Nuvem

- **Modelo baseado em consumo**

Os provedores de serviços de nuvem operam em um modelo baseado em consumo, o que significa que os usuários finais só pagam pelos recursos que usam. O que for usado é o que eles pagam.

  1. Melhor previsão de custos; 
  2. São fornecidos os preços para serviços e recursos individuais;
  3. A cobrançaé baseada no uso real.

- **Pizza as A Service/Pizza como serviço**

![image](https://user-images.githubusercontent.com/86172286/193891560-e24531a4-b4fb-4949-b690-8516e2fc73d2.png)


- **Infraestrutura como serviço (IaaS)**

Criar uma infraestrutura de TI de pagamento conforme o uso alugando servidores, máquinas virtuais, armazenamento, redes e sistemas operacionais de um provedor
de nuvem.

