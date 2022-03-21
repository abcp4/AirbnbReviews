# Airbnb Reviews


a. Como foi a definição da sua estratégia de modelagem?

**R: Escolhi abordar uma estratégia puramente em NLP, ignorando as demais variáveis categóricas. Utilizo modelos apropriados para texto como Bag of words, LSTM com attention e Transformers. Foram feitas duas tarefas: regressão da variável * e classificação de comentário bons e ruins**

b. Como foi definida a função de custo utilizada?
**R:Para regressão linear foi utilizada o Mean Squared Error(MSE)**

c. Qual foi o critério utilizado na seleção do modelo final?
**R:Os melhores resultados do MSE para a regressão, e o melhor f1 score para a classificação **

d. Qual foi o critério utilizado para validação do modelo? Por que escolheu utilizar este
método?
**R:Escolhi a predição do dataset na partição de validação, e também a visualização  das predições ordenadas em gráfico, por ser mais intuitivo para se observar a performance em casos não vistos pelo modelo.**

e. Quais evidências você possui de que seu modelo é suficientemente bom?
**R:Foi feita uma comparação entre modelos, dentre eles baselines como bag-of-words com modelos de regressão linear. O modelo de melhor performance foi o LSTM+Atenção, o que nos dá uma confiança de que ele é ao menos melhor que o baseline. Para a tarefa de classificação, avaliamos o entendimento do melhor modelo(Transformer) por meio de uma técnica de explicabilidade, o shap values.**
