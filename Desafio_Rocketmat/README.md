# Rocketmat <br />
### Processo seletivo para Estágio em Data Science <br />

Glauco Endrigo Moura de Lima

Email: glauco.endrigo@hotmail.com

Data: 05/09/2020  

* [Link do dataset:](https://www.kaggle.com/krismurphy01/data-lab)

## Tabela de conteúdo

* [Objetivo](#Objetivo)

<!-- Objetivo -->
#### Objetivo:

1. Fazer  uma análise do dataset e nos explicar  quais as principais informações e como
elas se relacionam. Deixar  claro quais as expectativas e quais as conclusões em cada passo da análise.

2. Enumerar  possíveis problemas que se pode resolver utilizando machine learning
neste dataset. Construir um ou mais modelos e nos mostrar habilidades de modelar um problema: decidindo features, labels e realizando uma experimentação. 

Problemas: 
1 -  Funcionários valiosos estão saindo prematuramente? Quais funcionários valiosos sairão em seguida ?. 



#### Descrição da base de dados:
| Variável                 | Descrição                                                    |
| ------------------------ | ------------------------------------------------------------ |
| ID                       | Identificador do funcionário                                 |
| Name                     | Nome                                                         |
| Department               | O departamento funcional ao qual o funcionário pertence.     |
| GEO                      | A geografia de trabalho à qual o funcionário pertence na organização matricial  |
| Role                     | A posição ou título do funcionário.                                             |
| Rising_Star              | Indica o nível de promessa ou capacidade de promoção do funcionário.            |
| Will_Relocate            | O funcionário está disposto a se mudar?                      |
| Critical                 | O funcionário é fundamental para a organização?              |
| Trending Perf            | Qual é a tendência de desempenho do funcionário este ano?    |
| Talent_Level             | Este campo representa um nível subjetivo da visão da administração sobre o funcionário|
| Validated_Talent_Level   | Esta visão da alta gerência de campo sobre o que o gerente declarou   |
| Percent_Remote           | Porcentagem de funcionários que trabalham remotamente.              |
| EMP_Sat_OnPrem_n         | indicador de uma pesquisa enviada aos funcionários. OnPrem significa que o funcionário mantém uma alta porcentagem de trabalho nos locais físicos de trabalho da empresa.                            |
| EMP_Sat_Remote_n         | indicador de uma pesquisa enviada aos funcionários. Remote (funcionário à distância) significa que o funcionário faz uma alta porcentagem do trabalho fora dos locais físicos de trabalho da empresa.|
| EMP_Engagement_n         | indicador de uma pesquisa enviada aos funcionários. Engagement representa o sentimento do funcionário sobre estar envolvido nas atividades da empresa                                        |
| last_evaluation          | A pontuação na última avaliação do funcionário                         |
| number_project           | Número de projetos em que o funcionário trabalha ao longo do ano       |
| average_montly_hours     | Número médio de horas que o funcionário trabalha                       |
| time_spend_company       | Anos de serviço                                                        |
| Work_accident            | Número de acidentes em que o funcionário está envolvido                |
| left_Company             | O funcionário saiu da empresa?                                         |
| CSR Factor               | Ignorar                                                                |
| promotion_last_5years    | O funcionário foi promovido nos últimos 5 anos?                        |
| sales                    | ignorar                                                                |
| salary                   | Grau salarial relativo (baixo, médio, alto) por função                 |
| Gender                   | Sexo ou como a pessoa se identifica                                    |
| LinkedIn_Hits            | O número de vezes que o funcionário visita sites de rede do LinkedIn.  |
| Emp_Work_Statusn         | Um indicador de uma pesquisa enviada aos funcionários por um terceiro. Status representa quão fortemente o funcionário se sente sobre seu nível de status na organização                                     |
| Emp_Identity             | Como o funcionário se identifica com a empresa.                                   |
| Emp_Role                 | Como o funcionário se identifica com a importância de seu papel na empresa.       |
| Emp_Position             | Como o funcionário se identifica com a importância de seu cargo na empresa.       |
| Emp_Title                | Como o funcionário se sente sobre seu título.                                     |
| Women_Leave              | Mulheres que saíram da empresa                                                    |
| Men_Leave                | Homens que deixaram a empresa.                                                    |
| Emp_Competitive_n        | Indicador de uma pesquisa enviada aos funcionários. Como o funcionário se sente sobre a natureza competitiva do trabalho na organização                                                                         |
| Emp_Collaborative_n      | Indicador de uma pesquisa enviada aos funcionários. Como o funcionário se sente sobre a natureza colaborativa do trabalho na organização                                                                        |
| Sensor_StepCount         | Sensores usados para capturar certas atividades dos funcionários. Neste caso, número de etapas      | Sensor_Heartbeat(Average/Min)         | Sensor de pulsação                                                   |
| Sensor_Proximity(1-highest/10-lowest) | Sensor de próximidade, o quão perto eles estão do laptop da empresa. |



#### Descrição dos arquivos: 

* HR_Engagement_Sat_Sales_UpdatedV4.0.csv - Dados do final da safra de 2018-2019.

Conjunto de dados analíticos de RH que pode ser usado para construir relatórios úteis, compreender a diferença entre dados e informações e análise multivariada. O conjunto de dados  é semelhante  aos  que podem ser encontrados nos subsistemas ERP RH.

Conteúdo:

Os campos representam um conjunto de dados fictício em que uma pesquisa foi realizada e existem métricas reais de funcionários para uma determinada organização. Nenhum desses dados são  reais.

Sobre este conjunto de dados. Analises sugeridas pelo 

Por os melhores e mais experientes funcionários estão saindo prematuramente? Tquais funcionários valiosos sairão em seguida ?. 

Os campos do conjunto de dados incluem:

* Nível de Satisfação
* Última avaliação
* Número de projetos
* Média de horas mensais
* Tempo passado na empresa
* Se eles tiveram um acidente de trabalho
* Se eles tiveram uma promoção nos últimos 5 anos
* Departamentos
* Salário

Para poder importar arquivos ipynb, use:
* pip install import-ipynb 

## Solução:

   # 1. Introdução
      1.1  Objetivo inicial
      1.2  Premissas
      1.3  Bibliotecas
    
   # 2. Análise inicial
      2.1 Ler o arquivo 
      2.2 Estatística básica
      2.3 Verificando os valores faltantes 
      2.4 Valores duplicados
      2.5 Considerações
        
   # 3 Análise exploratória de dados (AED)
      3.1 Pré-processamento inicial
      3.2 Mapa de correlação
      3.3 Coeficiente de Correlação de Pearson
      3.4 Distribuição de valores
      3.5 Criando features
      3.6 Gráficos de dispersão
      3.7 Gráficos de violino
      3.8 Histogramas - Escala logarítmica
      3.9 Inspeção visual - Histogramas
      3.10 Criando um dicionário de features
    
   # 4. Solução Machine Learning
      4.1 Melhores funcionários de acordo com a métrica "last_evaluation".


