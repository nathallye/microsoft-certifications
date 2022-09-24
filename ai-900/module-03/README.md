# AI-900: Azure AI Fundamentals

## Módulo 3: Pesquisa Visual Computacional

- **Conceitos de Pesquisa Visual Computacional**

  - **O que é Pesquisa Visual Computacional?**
    - Como o computador enxerga o mundo externo? Imagens, Câmera, Vídeos... Todo pixel da imagem é traçado ente 0 e 255. RGB 0 mais próximo de uma escala sem cor e 255 mais próximo do branco.
    
    ![image](https://user-images.githubusercontent.com/86172286/192073706-571719b7-a3ef-49ca-96c7-e89f443dbb8f.png)
 
   - Depois de classificar entre 0 a 255 o computador vai aplicar uma camada de rgb na imagem.
   O sistema de cores RGB é encontrado em monitores de computador, televisão, câmeras digitais entre outros. As cores são atingidas com a mistura das três cores primárias em um número definido numa escala de 0 a 255. Na mistura das três o valor máximo (255) atinge a cor branca e o valor mínimo (0) resulta na cor preta.
    
   ![image](https://user-images.githubusercontent.com/86172286/192073793-13907485-3605-420e-9a70-c51eae29640e.png)

- **Aplicag6es da Pesquisa Visual Computacional**
  - **Classificão de imagem** 
  - **Deteccaéo de Objetos**
  - **Segmentação semântica**
  - **Análise de imagem**
  - **Detecção e reconhecimento facil**
  - **Reconhecimento óptico de carcteres (ORC)**
  
  ![image](https://user-images.githubusercontent.com/86172286/192073936-47d90f61-9e44-4b31-87ae-b6308a91d584.png)

- **Serviços Cognitivo**
  1. Pesquisa Visual Computacional
  2. Moderador de conteúdo
  3. Rosto
  4. Reconhecimento de Formulários do Azure
  5. Visão personalizada
  6. Compreensão da Linguagem
  7. Fala
  8. Análise de texto
  9. Tradutor
  10. Indexador de video
  
  ![image](https://user-images.githubusercontent.com/86172286/192074037-6af61c56-fc00-4f1e-8b28-325097a3588b.png)

- **Análise de imagens com o servico de Pesquisa Visual Computacional**
  - Modelo de pesquisa visual computacional pré-treinado;
  - Detecção de objetos para mais de 10 mil classes predefinidas;
  - Descrição de imagem e geração de tags;
  - Detecçaão e análise facial;
  - Moderação de conteúdo;
  - Detecção de texto e OCR.
  
  ![image](https://user-images.githubusercontent.com/86172286/192074116-fbbf5551-eedc-4ba6-adb8-17e4dc36a604.png)

  Ex.: Detecção de público que passa em determinado local, para segmentar propagandas.

- **Treinamento de modelos com o servic¢o de Visdo Personalizada**
  Treinar o modelo com imagens e depois ele vai conseguir detectar esse objeto.
  Pode ser usado para treinar um modelo com fotos de um suspeito, para depois detectar ele através de câmeras de segurança, monitoramento...
  
  ![image](https://user-images.githubusercontent.com/86172286/192074250-e3696927-4bb5-48ef-be7d-f81de376ad58.png)

- **Análise de rostos com o serviço de Detecção Facial** 
  - Mais funcionalidades de análise facial do que o servico de Pesquisa Visual Computacional, entre elas:
    - Atributos faciais:
      - Idade
      - Emoção
    
    - Reconhecimento facial:
      - Combinação de similaridade
      - Verificacão de identidade

  ![image](https://user-images.githubusercontent.com/86172286/192074319-d10f1ebb-e168-441e-9539-1227a2d6a5fd.png)

- **Leitura de textos com o serviço de Pesquisa Visual Computacional**
  - Detectar a localização do texto:
    - Impresso
    - Manuscrito
  
  - Opções para extração rápida de texto de imagens ou análise assíncrona de documentos escaneados maiores.
  
  ![image](https://user-images.githubusercontent.com/86172286/192074443-8e5e5752-a8e9-406b-901d-ee1b03bb83fc.png)

- **Análise de formulários com o serviço de Reconhecimento de Formulários**
  - Extrair informações de formulários escaneados em formato de imagem ou PDF
    - Treinar um modelo personalizado usando seus prÓprios formulários
    - Usar o modelo de recibo pré-treinado
  - Os modelos realizam o reconhecimento semântico de campos de formulários, não só a extração de texto.
  
  Leitura de chave valor.
  
  ![image](https://user-images.githubusercontent.com/86172286/192074526-68b8a89e-8d0c-4354-ab11-a13f2956f81e.png)
