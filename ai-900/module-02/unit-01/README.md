# AI-900: Azure AI Fundamentals

## Módulo 3: Machine learning

- **O que é machine learning?**
Criação de modelos preditivos encontrando relações nos dados. Lições aprendidas. Ação baseada em grande volume de dados.

  - **Modelo de regressão(modelo de Machine learning supervisionado)**
    Temos como exemplo uma négocio de aluguéis de bicicletas, onde através de dados coletados temos a media de bicicletas alugadas de acordo com a temperatura. 
    Na validação temos uma variação em relação ao que a máquina foi treinada.
    Então o resultado da regração foi, com 54°F imaginavamos alugar 114 bicicletas e foram alugadas 116... então a curva de variação pode ser tanto para baixa quanto para cima.
    
    ![image](https://user-images.githubusercontent.com/86172286/191862510-2c388209-7e72-4c4f-979e-22f90e5741ef.png = 50x)
    
   - **Modelo de classificação(modelo de Machine learning supervisionado)**
    Mais complexo, tem muito falso positivo e a ideia é sempre trazer o falso positivo.
    Mais próximo de 1 é verdade e mais próximo de 0 é falso.
    
    ![image](https://user-images.githubusercontent.com/86172286/191863420-907a4806-957e-4262-add1-b91405b69d97.png)

    ![image](https://user-images.githubusercontent.com/86172286/191863655-14cc627f-6b2c-4d5b-a939-526d3750d4ab.png)

   - **Modelo de clustering(modelo de Machine learning não supervisionado - deixa a máquina trabalhando até chegar no resultado)**
    Agrupar elementos por características semelhantes.
    
    ![image](https://user-images.githubusercontent.com/86172286/191864063-ad9df58e-7f05-4eba-ae7d-3c0a71ec3752.png)

- **O que é o Azure Machine Learning?**
  Uma plataforma baseada em nuvem para machine learning. Assinatura do Azure. Plataforma.
    - Computação;
    - Dados;
    - Experimentos;
    - Modelos;
    - Serviços.
 
  ![image](https://user-images.githubusercontent.com/86172286/191864436-85385503-0fd8-4d46-900a-493a0a7da9d7.png)

- **Machine learning automatizado**
  - Elimina o trabalho árduo do machine learning
    - Forneça os dados e o tipo de modelo desejado e deixe o Azure Machine Learning encontrar o melhor modelo.

  - Bom para quem está começando.
  
  ![image](https://user-images.githubusercontent.com/86172286/191864756-283fd579-2747-43cd-b1b3-aa7f74dd7625.png)

- **Designer do Azure Machine Learning**
  Ferramenta visual para criação de um pipeline de machine learning.
  
  1. Use um pipeline de treinamento para treinar e avaliar um modelo;
  2. Crie um pipeline de inferência para prever etiquetas a partir dos dados novos;
  3. Implante o pipeline de inferência como serviço para uso nos aplicativos.

  ![image](https://user-images.githubusercontent.com/86172286/191865103-463db1f0-e567-4860-a571-c71db46afb1d.png)
