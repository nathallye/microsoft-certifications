# AI-900: Azure AI Fundamentals

## Módulo 3: Machine learning

- **O que é machine learning?**
Criação de modelos preditivos encontrando relações nos dados. Lições aprendidas. Ação baseada em grande volume de dados.

  - **Modelo de regressão(modelo de Machine learning supervisionado)**
    Temos como exemplo uma négocio de aluguéis de bicicletas, onde através de dados coletados temos a media de bicicletas alugadas de acordo com a temperatura. 
    Na validação temos uma variação em relação ao que a máquina foi treinada.
    Então o resultado da regração foi, com 54°F imaginavamos alugar 114 bicicletas e foram alugadas 116... então a curva de variação pode ser tanto para baixa quanto para cima.
    
    ![image](https://user-images.githubusercontent.com/86172286/191862510-2c388209-7e72-4c4f-979e-22f90e5741ef.png)
    
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
