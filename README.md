# Challenge_BI_Hive_Minsait_2023
Business Intelligence final challenge from Minsait training


Proposta: formação completa de um trabalho de Business Intelligence, usando 
  . GitHub como local de armazenamento/histórico, 
  . Gitpod e Jupyter Notebook como notebooks online, 
  . Docker para rodar o que for necessário, 
  . Shell scrips para automatizar subida de arquivos e demais atividades repetitivas,
  . Hive para colocar dados em hdfs, 
  . Power BI para criar visualizações gráficas dos dados.

Enunciado
  Atividade Desafio Final
Prof Caiuá França
•
31 de mar.
100 pontos
Data de entrega: 8 de abr.
efetuar o download do arquivo abaixo e enviar para pasta input do projeto de vocês

### **** Instruções **** ####

DESAFIO BIG DATA/BI

📌 ESCOPO DO DESAFIO
Neste desafio serão feitas as ingestões dos dados que estão na pasta /raw onde vamos ter alguns arquivos .csv de um banco relacional de vendas.

 - VENDAS.CSV
 - CLIENTES.CSV
 - ENDERECO.CSV
 - REGIAO.CSV
 - DIVISAO.CSV

Seu trabalho como engenheiro de dados/arquiteto de BI é prover dados em uma pasta desafio_curso/gold em .csv para ser consumido por um relatório em PowerBI que deverá ser construído dentro da pasta 'app' (já tem o template).

📑 ETAPAS
Etapa 1 - Enviar os arquivos para o HDFS
    - nesta etapa lembre de criar um shell script para fazer o trabalho repetitivo (não é obrigatório)

Etapa 2 - Criar o banco DEASFIO_CURSO e dentro tabelas no Hive usando o HQL e executando um script shell dentro do hive server na pasta scripts/pre_process.

    - DESAFIO_CURSO (nome do banco)
        - TBL_VENDAS
        - TBL_CLIENTES
        - TBL_ENDERECO
        - TBL_REGIAO
        - TBL_DIVISAO

Etapa 3 - Processar os dados no Spark Efetuando suas devidas transformações criando os arquivos com a modelagem de BI.
OBS. o desenvolvimento pode ser feito no jupyter porem no final o codigo deve estar no arquivo desafio_curso/scripts/process/process.py

Etapa 4 - Gravar as informações em tabelas dimensionais em formato cvs delimitado por ';'.

        - FT_VENDAS
        - DIM_CLIENTES
        - DIM_TEMPO
        - DIM_LOCALIDADE

Etapa 5 - Exportar os dados para a pasta desafio_curso/gold

Etapa 6 - Criar e editar o PowerBI com os dados que você trabalhou.

No PowerBI criar gráficos de vendas.
Etapa 7 - Criar uma documentação com os testes e etapas do projeto.

REGRAS
Campos strings vazios deverão ser preenchidos com 'Não informado'.
Campos decimais ou inteiros nulos ou vazios, deversão ser preenchidos por 0.
Atentem-se a modelagem de dados da tabela FATO e Dimensão.
Na tabela FATO, pelo menos a métrica <b>valor de venda</b> é um requisito obrigatório.
Nas dimensões deverá conter valores únicos, não deverá conter valores repetidos.

INSTRUÇÕES
vocês deveram me entregar o projeto no github e por email (zip)
