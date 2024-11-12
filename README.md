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


<strong> Calculando médias, medianas e moda</strong>

Utilizando o MEAD, MEDIAN e MODE foi realizado o cálculo da MÉDIA, MEDIANA e MODA das horas de sono para cada uma das profissões:

![Screenshot_95](https://github.com/user-attachments/assets/ccba8773-14bf-4528-8ff5-bbfb7154e092)


<strong>Com esses cálculos de média, mediana e moda foram realizadas algumas análises que ajudaram na resolução de questões, como:</strong>

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

<strong> Conclusões</strong>

<strong><li>De acordo com os dados, advogar ou ser representante de vendas faz você dormir menos?</li></strong>
<br>
É possível verificar que a profissão representante de vendas possui a menor média , mediana e moda e portanto é a profissão que menos dorme dentre todas, inclusive em relação ao advogado que possui a maior média de horas de sono segundo a análise. Com base nesses dados pode-se pensar em medidas para melhorar a qualidade de sono desses profissionais, talvez repensando a escala e volume de trabalho por colaborador ou ainda realizar outras análises e pesquisas que nos forneça mais informações do por quê. 

<strong><li>Quem tem maior pressão sanguínea média, homens ou mulheres?</li> </strong>

![Screenshot_96](https://github.com/user-attachments/assets/51353050-f4c6-40da-9299-b423d6e5076a)

![Screenshot_97](https://github.com/user-attachments/assets/708c2344-88ff-4aac-a514-62fb73d64560)
![Screenshot_98](https://github.com/user-attachments/assets/f3a32162-0d2f-4f12-b734-6327841b0036)

A coluna de Pressão Sanguínea continha os valores da pressão sistólica(PS) e diastólica(PD) na mesma coluna. Esses dados foram divididos em duas colunas e depois foi calculada a média dada pela inserção da coluna PAM (PS + 2 x PD)/3. Ao comparar a média da PAM para homens e mulheres, foi verificado que é maior nas mulheres. 

Também foi comparada a pressão arterial média por gênero e profissão. Repare também que há profissões que não é possível comparar por gênero pois só há mulheres ou homens. 

Como a diferença entre as médias entre os gêneros não é muito grande, não justifica medidas específicas para o grupo. Mas caso fosse, poderia sugerir que medidas como programas institucionais de promoção da saúde e bem estar voltado para mulheres, entre outras. Pode também ser voltado às mulheres da profissão que apresenta maior pressão arterial média, no caso, enfermeiras.

<strong><li>Pessoas com frequências cardíacas acima de 70 dão mais passos que pessoas com frequência cardíaca menor ou igual a 70?</li> </strong>

Comparando as médias, é possível verificar que as pessoas com frequência cardíaca acima de 70 dão menos passos que as com frequência menor ou igual a 70. Isso é um indicativo que caminhadas pode impactar positivamente na saúde cardíaca das pessoas podendo também relacionar esses dados com outros indicativos de bem estar como redução de estresse e melhora na circulação sanguínea. Isso também pode servir de base para programas de incentivo a caminhadas, uso de escadas em vez de elevadores, entre outros. 

