# StackLabs-Minio-Olist
**O objetivo desse repositorio é organizar os arquivos produzidos no desenvolvimento do projeto do [StackLabs](https://github.com/HenriqueSantos0/StackLabs-Minio-Olist/blob/main/Projeto%20-%20Stack%20Labs.pdf) da squad Minio.**
**Trata-se de um projeto End-to-End**

## Descrição
- A equipe desenvolveu, a partir de técnicas de Data Science, um modelo de **Previsão de vendas para as regiões Norte, Nordeste e Centro-Oeste do Brasil**, partindo do algorítimo Prophet do Facebook.
- O projeto proposto enquadra-se no tópico **Análise de dados e Entendimento de Negócio**. 
- As bases de dados da companhia foram utilizadas para a produção de um relatório, que concentra-se na exploração e análise de dados e no desenvolvimento de modelo preditivo de Manchine Learning, para a identificação de oportunidades.

## Problema
- Tentamos com esse projeto responder a seguinte pergunta: Que fatores permitem a manutenção do faturamento da companhia em acensão?
- Para isso, após análise exploratória dos dados trouxemos algumas informações para justificar o nosso estudo de caso.
1. Considerado o recorte temporal entre 2017 e 2018, as vendas anuais da empresa cresceram 18%, e o número de vendedores, 33%;
2. Os dados disponibilizados pela companhia demostram que mais de 70% dos pedidos foram entregues no eixo Sul-Sudeste. A duas regiões possuie densa rede de transporte, o que  explica o valor de frete menor, se comparado com regiões mais distantes do país;
3. A partir destes dados, verifica-se, portanto, que a distribuição de vendedores e vendas nos estados é irregular: o estado de SP concentra, por exemplo, 60% dos vendedores e 40% do faturamento da companhia.
<br>
<div align='center'>
<image src = "https://user-images.githubusercontent.com/89212899/151978158-16452e70-82c5-43ce-b232-b89f523f527b.png" width='800px'/>
</div>

<div align='center'>
<image src = "https://user-images.githubusercontent.com/89212899/151978197-07e7ab4e-f6c6-4a90-a663-2b89ba09ce3f.png" width='800px'/>
</div>

<div align='center'>
<image src = "https://user-images.githubusercontent.com/89212899/151978229-6cd7ac1e-d784-420e-a7d3-cf06bd8f731d.png" width='800px'/>
</div>

<div align='center'>
<image src = "https://user-images.githubusercontent.com/89212899/151978252-629c8e58-b037-412c-99a3-5fd5c1125781.png" width='800px'/>
</div>

## Hipótese de trabalho:
Para responder a questão de que *fatores permitem a manutenção do faturamento da companhia em acensão?* formulou-se a seguinte hipótese:

- O aumento do número de vendedores nos estados das regiões Norte, Nordeste e Centro-Oeste induziria a uma redução 1) de tempo de entrega de encomendas e 2) valor do frete, aumentado o volume de vendas nessas regiões;

## Solução de Engenharia de dados:

A solução para o armazenamento, seleção de features e análises foram foram desenvolvidas a partir do servico de cloud da Google, explicitado no diagrama abaixo:

<div align='center'>
<image src = "https://user-images.githubusercontent.com/48441841/152534708-e674780f-e32c-45e3-968f-9d929633d63b.png" width='500px'/>
</div>

## Modelos de previsão

1) Modelo de treino com resultados nacionais.

![image](https://user-images.githubusercontent.com/89212899/151978392-d521fc1c-c4cf-4cf3-8569-174aaab404c0.png)

2) O modelo de previsão paras as regiões analisadas demonstrou solidez, uma vez que as projeções de produtos vendidos são naturalemnte ascendentes. A métrica do RMSE demontrou uma variação de 28 erros padrão, o que demonstra uma baixa variação dessa previsão para um perído de 4 anos.

![image](https://user-images.githubusercontent.com/89212899/151978423-069f1bcd-2377-422a-a18f-d45bfb70f621.png)

