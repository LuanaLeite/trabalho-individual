# Introdução a Data Science - Trabalho em Individual realizado para a disciplina de Tópicos Especiais em Marketing II

Objetivo do trabalho: o objetivo geral do TI é desenvolver um projeto completo de data science, conforme roadmap visto na aula 1, com tema de livre escolha. 

**A empresa**: vende produtos de emagrecimento via canais digitais. Conta com uma audiência de mais de 6M de inscritos no Youtube e, aproximadamente, 980mil seguidores no Instagram. Além da produção de conteúdo orgânico, utilização de estratégias de lançamento de produto, a empresa também investe cerca de R$800 mil reais em tráfego pago por mês para captação de leads. 

**Problemática:** a empresa está no mercado desde 2019 e, recentemente, vem enfrentando novos desafios em relação ao custo de aquisição de clientes e redução de margem de lucro. Dado esse cenário, a grande pergunta feita pelo principal gestor da empresa, demandante da análise, foi "*Quem são os nossos melhores clientes? O que eles compraram?*".   

Além disso, a empresa acredita que seus melhores clientes possuem entre 45 e 54 anos. 

**O QUE DEFINE "MELHORES CLIENTES?**
Para definir quem são os melhores clientes da empresa, levando em consideração a problemática levantada, chegou-se a conclusão que seriam aqueles que, ao longo do tempo, aumentaram o valor gasto nos produtos da empresa. Para metrificar essa informação, utilizou-se o conceito de Live Time Value (LTV).
Para responder a pergunta feita pelo gestor da empresa, foi disponibilizada uma base de vendas histórica de janeiro de 2020 até novembro de 2022. A base é constituída do histórico de 5 plataformas de vendas (hotmart, guru-info, guru-sup, upnid e nutlog). Para organização e manipulação dos dados, tudo foi concatenado em excel, com trativas específicas para deixar as bases no mesmo formato e padronizar seus campos. 

**Informações disponibilizadas**
Foi disponibilizada uma base de vendas histórica de janeiro de 2020 até abril de 2023. A base é constituída do histórico de 5 plataformas de vendas (hotmart, guru-info, guru-sup, upnid e nutlog). Para organização e manipulação dos dados,  tudo foi concatenado em excel, com trativas específicas para deixar as bases no mesmo formato e padronizar seus campos. 

Uma base chamada "pesquisa" foi agregada ao histórico de vendas. Essa base contém informações acerca do perfil do cliente como, por exemplo, idade, gênero, renda, escolaridade, entre outras.

Para melhor compreensão da base extraída para análise, confira o **dicionário de variáveis**: https://docs.google.com/spreadsheets/d/1h7uDHroNP6_lTfM1Is5HvlHgBBAP84sNmIXJD1hWgEo/edit?usp=sharing

**COLETA E PRÉ-PROCESSAMENTO**
- Foi necessário realizar ajustes de padronização, tratamento de formatação de variáveis como textos, números e datas. 
- O calculo do LTV foi realizado com base no total de compras feitas ao longo do tempo multiplicado pelo valor da compra. 
- Variáveis categóricas foram transformadas em variáveis dummies e inseridas no dataframe. 

**RESULTADOS**

**Idades que mais influenciam no LTV:** clientes das faixas entre 55 e 64 anos e 65 anos ou mais, desvalidando a premissa do gestor da empresa que os melhores clientes estão entre 45 e 54 anos.

**10 produtos comprados pelos melhores clientes** 
 VitaCalm Night - Kit com 3 Potes  (Melatonina)  
Revista Digital: Viva com Saúde por Dr. XXX...  
Colágeno Tipo 2 | Kit 90 dias  
Vitacongress - Plano Diamante  
Fórmula SB3 - Kit com 3 Potes  
[VSA] Viva com Saúde (Assinatura)  
Multivita Women (Mulheres) - Kit com 3 Potes  
 Ômega Vita - Pote Unitário (Frete grátis)  
Fórmula SB4 - Pote Unitário  
Multivita Mulheres  

**LIMITAÇÕES DO PROJETO**
Tamanho da base vs Informações disponíveis: apesar da base conter um grande número de informações (193 mil registros), apenas 50 mil possuiam dados específicos do cliente. 

Observações nulas: muitos registros precisaram ser adaptados para a aplicação do modelo, o que reduz sua confiabilidade.

Baixo desempenho dos modelos: os modelos testados com as variáveis independentes disponíveis tiveram baixo desempenho para explicar a variável dependente.

