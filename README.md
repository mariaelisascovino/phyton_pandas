# phyton_pandas
Phyton Pandas

Uso de Python com a biblioteca Pandas. Análise do dataframe em csv sobre saúde do sono.

- Visualização do dataframe;
- Filtragem de dados;
- Tratamento de dados;
- Cálculo de médias, modas e medianas;
- Edição e conversão de dados.

DATAFRAME SOBRE DISTÚRBIOS DO SONO

O dataframe analisado reúne informações de pessoas com suas ocupações, dados pessoais e médicos como idade e pressão sanguínea e uma coluna que traz a informação de distúrbio de sono dividida em 3 categorias: apnéia do sono, insônia e nenhuma. 

Ele possui 373 linhas e 13 colunas e não possui valores nulos.

LEITURA INICIAL DO DATAFRAME:

![Screenshot_68](https://github.com/user-attachments/assets/f67c2ac6-5d65-4579-9601-fdc87df7e878)


Após a leitura do arquivo no Google Colab e nomeando o dataframe como df_saude_do_sono_estilo_vida foram feitas algumas análises:

<strong>Renomeando algumas colunas para melhor identificação:</strong>

Utilizando o método RENAME foram renomeadas as colunas ID, Pressão sanguíneaaaa, Ocupação, Categoria BMI para Identificador, Pressão Sanguínea, Profissão e Categoria IMC.

![colunas](https://github.com/user-attachments/assets/d59ad02d-934d-40d2-9847-bfd61ff7d1cd)

<strong> Contagem de dados </strong>

Utilizando o método COUNT foi levantado o dado de número de pessoas por profissão:

![quantidade_prof](https://github.com/user-attachments/assets/61770d94-b9ce-4111-9e34-04352152500a)


<strong> Calculando médias, medianas e moda<strong>

Utilizando o MEAD, MEDIAN e MODE foi realizado o cálculo da MÉDIA, MEDIANA e MODA das horas de sono para cada uma das profissões:

![med](https://github.com/user-attachments/assets/b2aa24c6-3f81-4221-a1da-b088b029e930)

Com esses cálculos de média, mediana e moda foram realizadas algumas conclusões que ajudaram na resolução de questões, como:

<ul><em>
<li>De acordo com os dados, advogar ou ser representante de vendas faz você dormir menos?</li> 
  
<li>Quem tem maior pressão sanguínea média, homens ou mulheres?</li> 
  
<li>Pessoas com frequências cardíacas acima de 70 dão mais passos que pessoas com frequência cardíaca menor ou igual a 70?</li> 

</em></ul>

<strong> Extraindo outras informações</strong>

Utilizando operadores aritméticos, filtragem por coluna e SHAPE foram extraídas informações do dataframe,tais como:

<ul><em>

<li>Das pessoas que atuam com engenharia de software qual a porcentagem de obesos?</li>

<li> Filtrar ou criar dataframe com apenas colunas específicas.</li>


</em></ul>
