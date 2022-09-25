# AI-900: Azure AI Fundamentals

## Módulo 5: IA conversacional

 - **Conceitos de IA conversacional**
  IA conversacional é muito voltada para bots.
  
  - **O que é IA conversacional?**
   - Uma solução que `possibilita o diálogo` entre um agente de IA e um ser humano;
   - Genericamente, os agentes de IA conversacional sao conhecidos como bots;
   - Os bots podem interagir em vários canais:
    - Interfaces de Webchat
    - Email
    - Plataformas de mídia social
    - Serviço de Voz

  ![image](https://user-images.githubusercontent.com/86172286/192123652-8b9ea2b0-58fe-4f9e-877d-265700555383.png)

 - **Diretrizes de IA responsavel para bots**
  1. Seja transparente em relagdo ao que um bot pode (ou nao) fazer;
  2. Deixe claro que o usuário está se comunicando com um bot;
  3. Habilite o bot para fazer a transferência automática para um humano, caso necessario;
  4. Garanta que o bot respeite as normas culturais;
  5. Verifique se o bot é confiavel;
  6. Respeite a privacidade do usuário(não pedir dados - máx primeiro nome da mãe, 3 primeiro número do CPF);
  7. Manipule os dados com segurança;
  8. Assegure que o bot atenda aos padrões de acessibilidade(tem que atender em LIBRAS, aúdio, e texto);
  9. Assuma a responsabilidade pelas ações do bot.

- **IA conversacional no Azure**
 - **O servico QnA Maker**
  - Defina uma base de dados de conhecimento de pares de pergunta e resposta:
   - Inserindo perguntas e respostas
   - A partir de um documento de FAQs existente
   - Usando um bate-papo integrado
  - Consuma a base de dados de conhecimento de aplicativos clientes, inclusive bots
 
 ![image](https://user-images.githubusercontent.com/86172286/192123848-f7060ac5-18fd-4538-ab29-6ea1cc0b6d1a.png)

 - **Servico de Bot do Azure**
  - Plataforma baseada em nuvem para desenvolver e gerenciar bots
  - Integração com LUIS, QnA Maker e outros
  - Conectividade em vários canais

 ![image](https://user-images.githubusercontent.com/86172286/192123853-a81a9a0e-d7c2-42c0-88b5-1c946262c604.png)
