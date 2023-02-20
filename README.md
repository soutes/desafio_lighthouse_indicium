Repositório para o desafio do Lighthouse Indicium Tech 2023

<h1>Introdução:</h1>
Este teste consiste em criar um modelo preditivo para um conjunto de dados de máquinas, onde seja possível prever quais máquinas apresentam potencial de falha.

<h1>Sobre o desafio</h1>
<h3>Desafio</h3>

Seu objetivo é identificar quais máquinas apresentam potencial de falha tendo como base dados extraídos através de sensores durante o processo de manufatura.  Para isso são fornecidos dois datasets: um dataset chamado desafio_manutencao_preditiva_treino composto por 6667 linhas, 9 colunas de informação (features) e a variável a ser prevista (“failure_type”). 

O segundo dataset chamado de desafio_manutencao_preditiva_teste possui 3333 linhas e 8 colunas e não possui a coluna “failure_type”. Seu objetivo é prever essa coluna a partir dos dados enviados e nos enviar para avaliação dos resultados.

Você poderá encontrar em anexo um dicionário dos dados.


<h3>Entregas</h3>

Descreva graficamente os dados disponíveis, apresentando as principais estatísticas descritivas. Comente o porquê da escolha dessas estatísticas.
Explique como você faria a previsão do tipo de falha a partir dos dados. Quais variáveis e/ou suas transformações você utilizou e por quê? Qual tipo de problema estamos resolvendo (regressão, classificação)? Qual modelo melhor se aproxima dos dados e quais seus prós e contras? Qual medida de performance do modelo foi escolhida e por quê?<br/>
Envie o resultado final do modelo em uma planilha com apenas duas colunas (rowNumber, predictedValues). <br/><br/>
A entrega deve ser feita através de um repositório de código público que contenha:<br/>
README explicando como rodar o projeto<br/>
Arquivo requirements com todos os pacotes utilizados<br/>
Relatório de EDA em PDF, Jupyter Notebook ou semelhante conforme passo 1<br/>
Códigos de modelagem utilizados no passo 2.<br/>
Arquivo final predicted.csv conforme passo 3 acima.


<h3>Sobre o conjunto de dados:</h3>
Para a etapa de treinamento foi fornecido um dataset chamado desafio_manutencao_preditiva_treino composto por 6667 linhas, 9 colunas de informação (features) e a variável a ser prevista (“failure_type”). 

O segundo dataset chamado de desafio_manutencao_preditiva_teste possui 3333 linhas e 8 colunas e não possui a coluna “failure_type” é o conjunto de dados utilizado no teste.

<h1>Estrutra do diretório:</h1>
<h3>Arquivos com os dados:</h3>
<b>desafio_manutencao_preditiva_treino.csv</b> - Base de dados para analise, visualização e tratamento dos dados e criação do modelo.
<b>desafio_manutencao_preditiva_teste.csv</b> – Base de dados para teste do modelo.
predicted.csv – Arquivo com os dados resultantes do teste aplicado ao modelo.

<h3>Arquivos criados em Jupyter notebook:</h3>
<b>teste_cd_lighthouse-OK.ipynb</b> – Este é o arquivo de analise, visualização e tratamento dos dados. No final do mesmo consta o modelo que apresentou a melhor acurácia.
OBS.: Fiz o teste com outros modelos, sendo que o XGBClassifier foi o que apresentou a segunda melhor acurácia, de 98,23%, pouco abaixo do modelo escolhido, o RandomForestClassifier que apresentou acurácia de 98,50% e por este motivo, foi o modelo utilizado nos testes.

<b>teste_novos_dados.ipynb</b> – Neste arquivo consta a importação do modelo exportado utilizando a biblioteca Pickle assim como a importação dos dados novos (desafio_manutencao_preditiva_teste.csv) para uma tabela. Após isso é feito o teste e depois um breve ajuste na tabela para gerar a tabela final conforme solicitada no desafio, a tabela com apenas duas colunas: índice e resultados do modelo aplicado.

<h3>Arquivos somente de visualização:</h3>
<b>teste_cd_lighthouse-OK - Jupyter Notebook.pdf <br/>
teste_novos_dados - Jupyter Notebook.pdf</b> <br/>
Estes dois arquivos são apenas para uma visualização rápida do conteúdo, gráficos e códigos dos arquivos criados no Jupyter Notebook. Nestes arquivos constam as respostas para o item 1 e 2 do desafio.

<h3>Demais arquivos</h3>
<b>RF_model.pickle</b> – Arquivo perpetuado do modelo.

<b>predicted.csv</b> – Arquivo com os resultados dos teste utilizando o modelo, conforme solicitado no desafio.

<b>requirements.txt</b> – Arquivo com os requerimentos do sistema, conforme solicitado no desafio.
