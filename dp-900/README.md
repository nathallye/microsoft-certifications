# DP-900: Microsoft Azure Data Fundamentals

## Módulo 1: Explorar os principais conceitos de dados

### Lição 1: Explorar os principais conceitos de dados

- Objetivos da lição 1:
  1. Identificar como os dados são definidos e armazenados;
  2. Identificar características de dados relacionais e não relacionais;
  3. Descrever e diferenciar cargas de trabalho de dados;
  4. Descrever e diferenciar dados de lote e de streaming.

- O que são dados?
Coleção de fatos, informação, números, descrições, objetos, armazenados de maneira estrruturada, semiestruturada, não estruturada. Esses dados servem para guiar a empresa/organização em determinadas tomadas de decisões ou até mesmo para trazer resultados em planejamentos, vendas...

![Capturar](https://user-images.githubusercontent.com/86172286/188035359-51784f45-dff2-44ad-a86e-3c4fd390f390.PNG)

- Tipos de dados:
  1. Estruturados: É o que a maioria dos devs estão acostumados a trabalhar. São banco de dados relacionais, onde temos ``tabelas`/tables, `colunas`/columns e `linhas`/rows;
  2. Semiestruturados: É o que devs de front-end estão mais habituados a trabalhar, que nada mais é que dados em objetos JSON, consumindo API's e trazendo esses dados. Podem ser percitidos em bancos de dados NoSQL/Não relacionais;
  3. Não estruturado: Pode ser um documento, uma foto, um áudio, um vídeo.
  
- Armazenamento de dados transacional x analítico:
Temos alguns formatos de armazenamento de dados, ou seja, transações de modelos de armazenamento. 
  1. Um deles é o `Transacional`, `Transações on-line` que é o `Online Transactions Processing/Processamento Transações Online(OLTP)`, nele podemos guardar arquivos que fazemos upload durante uma transação, uma tabela armazenando cliente e pedidos desse cliente(banco de dados transacional).
  2. E outro é o `Analítico`  que é o `Online Analytic Processing/Processamento Analítico Online(OLAP)`, que ficou muito famoso no começo da década de 2000 por ser um processamento em lote e depois era transportado para alguma ferramenta de analytics e gerava insights com gráficos.

![Capturar1](https://user-images.githubusercontent.com/86172286/188037195-2212c8c4-2175-4fbc-8934-a8c90b51e6d8.PNG)

**Pergunta:** Temos uma solução hoje que precisamos guardar as informações de cada venda(quem é o cliente, qual foi o produto, preço)... onde armazenamos isso? Em um `OLTP - Online Transactions Processing` ou em um `OLAP - Online Analytic Processing`?
**Resposta:** OLTP, porque estamos armazenando cada item.
Se no final do dia precisássemos processar o lote de transações ou de vendas faria todo sentido realizar um OLAP para extrair no final do dia e/ou final do mês o volume de dados/informações e levar para o cubo/alguma ferramenta de analytics e gerar insights com gráficos.

- Quando fazemos transações `OLTP - Online Transactions Processing/Processamento Transações Online` precisamos seguir algumas informações, como por exemplo, `Cargas de trabalho transacionais`:
Os dados transacionais são informações que rastreiam as interações relacionadas às atividades de uma organização.
  1. **Atomicidade:** cada transação é tratada como uma unidade independente que resulta em sucesso completo ou falha completa;
  2. **Consistência:** as transações só podem conduzir os dados do banco de dados de um estado válido para outro estado válido;
  3. **Isolamento:** a execução concorrente de transações deixa o banco de dados no mesmo estado;
  4. **Durabilidade:** assim que uma transação tiver sido confirmada, permanecerá assim.
    
    
