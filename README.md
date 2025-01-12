# Analise-e-Previsao-de-Renda-com-base-em-Dados-Demograficos

##Introdução:

Este projeto tem como objetivo analisar um conjunto de dados demográficos para entender os fatores que influenciam a renda de um indivíduo e construir um modelo preditivo para estimar se a renda de uma pessoa será maior ou menor que 50 mil dólares por ano.

## Análise da Imagem e Código: Uma Tradução Detalhada

![cl0](https://github.com/user-attachments/assets/52fddee2-b215-4b10-8f99-3dcbbef10404)

**Código:**

O código Python fornecido realiza as seguintes tarefas:

1. **Seleção de Dados:**
   - `df = data[data['income'] == '>50K']`: Essa linha cria um novo DataFrame (df) filtrando os dados originais (data) para incluir apenas as linhas onde a coluna 'income' tem o valor '>50K'. Em outras palavras, seleciona apenas os indivíduos com renda superior a 50K.

2. **Agrupamento e Contagem:**
   - `agrupado = df.groupby(['sex'])['income'].count()`: Essa linha agrupa o DataFrame filtrado (df) pela coluna 'sex' (gênero), contando o número de ocorrências de cada nível de renda em cada grupo de gênero. O resultado é armazenado na variável agrupado.

3. **Criação do Gráfico de Pizza:**
   - `agrupado.plot.pie()`: Essa linha gera um gráfico de pizza usando os dados agrupados (agrupado). Cada fatia do gráfico representa um grupo de gênero, e o tamanho da fatia corresponde à proporção de indivíduos nesse grupo com renda superior a 50K.

**Insights:**

- **Distribuição de Renda:** O gráfico de pizza visualiza como a proporção de indivíduos com renda superior a 50K varia entre homens e mulheres.
- **Possível Desigualdade de Gênero:** O tamanho das fatias no gráfico de pizza pode indicar uma possível desigualdade de gênero nos níveis de renda. Se uma fatia for significativamente maior que a outra, sugere que um gênero tem uma proporção maior de indivíduos com renda superior a 50K.
- **Foco da Análise:** O código e o gráfico demonstram um foco específico na análise dos níveis de renda para indivíduos com ganhos superiores a 50K, provavelmente para explorar a desigualdade de renda ou outros fatores relevantes.

![cl1](https://github.com/user-attachments/assets/13764cef-561e-4d5c-a6f0-5e6e01b808fa)

**Código:**

O código Python fornecido executa as seguintes etapas:

1. **Seleção de Dados:**
   - `df1 = data[data['income'] == '<=50K']`: Essa linha cria um novo conjunto de dados (df1) filtrando o conjunto de dados original (data) para incluir apenas as linhas onde a coluna 'income' tem o valor '<=50K'. Em outras palavras, seleciona apenas os indivíduos com renda igual ou inferior a 50K.

2. **Agrupamento e Contagem:**
   - `agrupado1 = df1.groupby(['sex'])['income'].count()`: Essa linha agrupa o conjunto de dados filtrado (df1) pela coluna 'sex' (gênero), contando o número de ocorrências de cada nível de renda em cada grupo de gênero. O resultado é armazenado na variável agrupado1.

3. **Criação do Gráfico de Pizza:**
   - `agrupado1.plot.pie()`: Essa linha gera um gráfico de pizza utilizando os dados agrupados (agrupado1). Cada fatia do gráfico representa um grupo de gênero, e o tamanho da fatia corresponde à proporção de indivíduos nesse grupo com renda igual ou inferior a 50K.

**Insights:**

Com base na imagem e no código, podemos extrair as seguintes informações:

- **Distribuição de Renda:** O gráfico de pizza mostra como a proporção de indivíduos com renda igual ou inferior a 50K se distribui entre homens e mulheres.
- **Possível Desigualdade de Gênero:** O tamanho das fatias no gráfico de pizza pode indicar uma possível desigualdade de gênero nos níveis de renda. Se uma fatia for significativamente maior que a outra, sugere que um gênero tem uma proporção maior de indivíduos com renda igual ou inferior a 50K.
- **Foco da Análise:** O código e o gráfico demonstram um foco específico na análise dos níveis de renda para indivíduos com ganhos iguais ou inferiores a 50K, provavelmente para explorar a desigualdade de renda ou outros fatores relevantes.

![cl2](https://github.com/user-attachments/assets/f1d04378-1bf3-4e8a-b812-e1773b8d8d3e)

### Gráfico
O gráfico de barras apresentado mostra a **relação entre o nível de escolaridade e a faixa salarial**. Ele compara a quantidade de pessoas com diferentes níveis de educação que ganham mais de 50 mil dólares por ano com aquelas que ganham 50 mil dólares ou menos.

### Insights

A partir do gráfico e da análise do código, podemos extrair os seguintes insights:

* **Educação e Renda:** Existe uma clara correlação entre o nível de educação e a renda. Pessoas com níveis de educação mais altos (como bacharelado, mestrado e doutorado) tendem a ter rendas mais elevadas.
* **Nível Médio:** O grupo com ensino médio completo ("HS-grad") apresenta o maior número de pessoas, mas uma parcela significativa deles tem renda igual ou inferior a 50 mil dólares.
* **Ensino Superior Incompleto:** O grupo de pessoas com "Some-college" (ensino superior incompleto) também possui um número considerável de indivíduos, com uma distribuição de renda mais variada.
* **Implicações:** Esses resultados sugerem que a educação é um fator importante para determinar a renda. Investir em educação e oferecer oportunidades de desenvolvimento de habilidades pode ajudar as pessoas a alcançar níveis de renda mais altos.

**Em resumo:**

O gráfico e o código demonstram a importância da educação na determinação da renda. Pessoas com níveis de educação mais altos tendem a ter rendas mais elevadas. No entanto, outros fatores também podem influenciar a renda, e é importante considerar essas nuances ao interpretar os resultados.

![cl3](https://github.com/user-attachments/assets/a7461c80-f4b0-4ddb-ad16-e7871ce03083)


### Gráfico
O gráfico de barras apresentado mostra a **relação entre o estado civil e a faixa salarial**. Ele compara a quantidade de pessoas em diferentes estados civis que ganham mais de 50 mil dólares por ano com aquelas que ganham 50 mil dólares ou menos.

As barras são empilhadas, onde a parte azul representa aqueles que ganham mais de 50 mil dólares e a parte laranja representa aqueles que ganham 50 mil dólares ou menos.


### Insights

A partir do gráfico e da análise do código, podemos extrair os seguintes insights:

* **Estado Civil e Renda:** Existe uma clara relação entre o estado civil e a renda. 
    * **Casados:** Homens casados ("Husband") apresentam uma proporção significativamente maior de pessoas com renda acima de 50 mil dólares.
    * **Mulheres Casadas:** Mulheres casadas ("Wife") também têm uma parcela considerável de pessoas com renda acima de 50 mil dólares, mas em menor proporção que os homens casados.
    * **Solteiros e Outros:** Os grupos de "Not-in-family", "Unmarried" e "Other-relative" tendem a ter uma proporção maior de pessoas com renda igual ou inferior a 50 mil dólares.
* **Implicações:** Esses resultados sugerem que o estado civil pode ser um fator que influencia os níveis de renda. No entanto, é importante ressaltar que o estado civil é apenas um dos muitos fatores que podem influenciar a renda, e outros fatores como educação, experiência profissional e setor de atividade também desempenham um papel importante.

### Análises Adicionais e Considerações

* **Análise Quantitativa:** Calcular as porcentagens exatas para cada estado civil e faixa salarial pode fornecer insights mais precisos sobre a relação entre as duas variáveis.
* **Outros Fatores:** É importante considerar outros fatores que podem influenciar a renda, como educação, ocupação, experiência, idade e gênero, em conjunto com o estado civil.
* **Limitações dos Dados:** Os resultados da análise se baseiam em um conjunto de dados específico e podem não ser generalizáveis para toda a população. É crucial considerar as limitações e possíveis vieses dos dados.

**Em resumo:**

O gráfico e o código demonstram que o estado civil está relacionado com a renda, com homens casados tendendo a ter rendas mais elevadas. No entanto, é importante considerar outros fatores e realizar análises mais aprofundadas para entender completamente essa relação.

## criando e treinando o modelo de classificaçao

![cl4](https://github.com/user-attachments/assets/7f0b8ba7-c2d2-416d-b625-0a1fc5a14362)


### O que o código faz?

O código Python fornecido realiza uma **análise de classificação** utilizando um modelo de **Regressão Logística**. O objetivo é prever se uma pessoa terá uma renda superior a 50 mil dólares por ano com base em diversas características, como idade, nível de educação, ocupação, etc.

**Passo a passo do código:**

1. **Preparação dos Dados:**
   * **Divisão dos dados:** Os dados são divididos em dois conjuntos: um para **treinamento** do modelo (80% dos dados) e outro para **teste** (20% dos dados).
   * **Definição das variáveis:** A variável `X` contém as características que serão utilizadas para fazer as previsões (features) e a variável `y` contém a variável que se deseja prever (a renda, que pode ser acima ou abaixo de 50 mil dólares).

2. **Criação e Treinamento do Modelo:**
   * **Criação do modelo:** É criado um modelo de Regressão Logística, que é adequado para problemas de classificação binária (sim ou não).
   * **Treinamento do modelo:** O modelo é "treinado" utilizando os dados de treinamento. O modelo aprende a identificar padrões nos dados que relacionam as características com a renda.

3. **Previsão e Avaliação:**
   * **Previsões:** O modelo treinado é utilizado para fazer previsões sobre os dados de teste.
   * **Avaliação:** A precisão das previsões é avaliada utilizando três métricas:
     * **Acurácia:** A proporção de previsões corretas.
     * **Recall:** A capacidade do modelo de identificar corretamente os casos positivos (pessoas com renda acima de 50 mil dólares).
     * **Precisão:** A proporção de previsões positivas que são realmente positivas.

### Interpretação dos Resultados

Os resultados mostram que o modelo de Regressão Logística alcançou uma acurácia de aproximadamente 80%, o que significa que ele acertou cerca de 80% das previsões. No entanto, a métrica de recall é relativamente baixa (cerca de 43%), indicando que o modelo pode estar tendo dificuldade em identificar corretamente as pessoas com renda acima de 50 mil dólares. Por outro lado, a precisão é moderadamente alta (cerca de 64%), o que sugere que quando o modelo prevê que alguém tem uma renda acima de 50 mil dólares, ele está certo na maioria das vezes.


**Em resumo,** o código demonstra como construir e avaliar um modelo de aprendizado de máquina para prever a renda de indivíduos com base em suas características. Os resultados obtidos indicam que o modelo tem um bom desempenho geral, mas pode ser aprimorado para obter melhores resultados em relação à identificação de pessoas com renda acima de 50 mil dólares.

![cl5](https://github.com/user-attachments/assets/b35a55d2-642f-48ef-a47d-59978b25f625)

**Interpretando a Matriz:**

Na imagem fornecida, a matriz de confusão mostra o desempenho de um modelo de classificação que prediz se uma pessoa terá uma renda acima ou abaixo de 50 mil dólares.

* **Verdadeiros Positivos (VP):** 4591 casos em que o modelo previu corretamente que a pessoa tem uma renda acima de 50 mil dólares.
* **Verdadeiros Negativos (VN):** 669 casos em que o modelo previu corretamente que a pessoa tem uma renda igual ou inferior a 50 mil dólares.
* **Falsos Positivos (FP):** 377 casos em que o modelo errou ao prever que a pessoa tem uma renda acima de 50 mil dólares, quando na verdade era inferior.
* **Falsos Negativos (FN):** 875 casos em que o modelo errou ao prever que a pessoa tem uma renda igual ou inferior a 50 mil dólares, quando na verdade era superior.

**O que o Código Faz?**

O código Python utiliza a biblioteca Seaborn para criar uma visualização da matriz de confusão. Ele:

1. **Calcula a matriz de confusão:** A função `confusion_matrix` compara as previsões do modelo com os valores reais.
2. **Cria o gráfico:**
   * **Figura:** Cria uma figura com um tamanho específico.
   * **Mapa de calor:** Cria um mapa de calor usando a biblioteca Seaborn, onde cada célula representa um valor da matriz de confusão.
   * **Eixos e rótulos:** Define os rótulos dos eixos x e y, indicando "Valores Previstos" e "Valores Verdadeiros", respectivamente.
   * **Título:** Adiciona um título ao gráfico para explicar o que ele representa.

**Insights:**

* **Desempenho do Modelo:** A matriz de confusão mostra que o modelo tem um bom desempenho na classificação de pessoas com renda inferior a 50 mil dólares (alto número de verdadeiros negativos). No entanto, o modelo tem mais dificuldade em classificar corretamente as pessoas com renda superior a 50 mil dólares (número relativamente alto de falsos negativos).
* **Análise de Erros:** A análise dos valores de falsos positivos e falsos negativos pode ajudar a identificar os tipos de erros que o modelo está cometendo. Por exemplo, um alto número de falsos positivos pode indicar que o modelo está classificando muitas pessoas como tendo renda alta quando na verdade não têm.
* **Melhorias:** Com base na matriz de confusão, podemos identificar áreas onde o modelo pode ser melhorado. Por exemplo, podemos tentar ajustar os hiperparâmetros do modelo, adicionar ou remover features, ou utilizar técnicas de balanceamento de classes para lidar com desequilíbrios nos dados.

# prevendo novos dados

![cl6](https://github.com/user-attachments/assets/668aa4c1-dbe0-473d-a2b8-3a5e32b309d9)


**O que o código faz?**

O código Python fornecido realiza uma série de etapas de pré-processamento de dados e, em seguida, utiliza um modelo de machine learning para fazer previsões. Vamos analisar cada parte:

1. **Seleção de Features:**
   - `teste = teste.iloc[:, 0:10].values`: Essa linha extrai as primeiras 10 colunas (características) do DataFrame 'teste' e as converte em um array NumPy. Essas 10 colunas serão utilizadas como entrada para o modelo de machine learning.

2. **Codificação de Variáveis Categóricas:**
   - `teste[:, 1] = label_enco.fit_transform(teste[:, 1])`: Essa linha, e as seguintes linhas semelhantes para outras colunas, aplicam uma técnica chamada "label encoding" às colunas selecionadas. Essa técnica converte valores categóricos (como "sim" ou "não") em valores numéricos, o que é necessário para a maioria dos algoritmos de machine learning.

3. **Previsão:**
   - `nova_previsao = modelo.predict(teste)`: Nesta linha, o modelo treinado (representado por `modelo`) é utilizado para fazer previsões sobre os dados pré-processados em `teste`. O resultado das previsões é armazenado em `nova_previsao`.

4. **Saída:**
   - `array([0, 0, 0])`: O resultado da previsão é um array de valores. Nesse exemplo específico, o modelo previu a classe 0 para todos os exemplos de teste. No entanto, sem mais contexto sobre o que representa a classe 0, é difícil dizer o significado exato dessas previsões.

**Insights:**

* **Pré-processamento:** O código demonstra a importância do pré-processamento de dados antes de aplicar um modelo de machine learning. A seleção de features e a codificação de variáveis categóricas são etapas cruciais para garantir que os dados estejam no formato correto para o modelo.
* **Modelo de Machine Learning:** O código assume a existência de um modelo treinado (`modelo`) que é utilizado para fazer as previsões. O tipo de modelo e os detalhes de seu treinamento não são fornecidos no código apresentado.
* **Interpretação das Previsões:** O resultado final (`array([0, 0, 0])`) indica as previsões do modelo para os dados de teste. que novos dados sao para acima de 50k















