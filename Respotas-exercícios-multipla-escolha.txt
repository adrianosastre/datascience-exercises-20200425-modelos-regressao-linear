Respostas dos Exercícios de múltipla escolha

1. Exercício 1 (Modelos de Regressão Linear Simples e Múltipla)
Sobre os conceitos relacionados ao modelo de regressão abaixo, marque a alternativa correta:
hq (x) = q0+q1x

( ) a) Trata-se de um modelo matemático não paramétrico conhecido como Kernel.
( ) b) Trata-se de um modelo matemático em que x consiste nos parâmetros de entrada, q0
e q1 são constantes e hq (x) é a variável de saída.
( ) c) Trata-se de um modelo de regressão linear em que q0 e q1 são parâmetros que
precisamos encontrar por meio do processo de treinamento do modelo.
(X) d) Trata-se de um modelo matemático em que x é uma constante de entrada unitária, q0
e q1 são valores aleatórios hq (x) é a variável de saída.

2. Exercício 2 (Modelos de Regressão Linear Simples e Múltipla)
A tabela abaixo apresenta um pequeno conjunto de dados que relaciona a variável explanatória
- tamanho (área) das casas com a variável de saída - preços de diversas casas,
formando os pares (x(i);y(i)). De acordo com a notação usada no curso para descrever o
conjunto de dados, marque a alternativa que o retrata corretamente:

(x) Área das casas (m2) Preços (em mil reais) (y)
    220                 180
    250                 200
    150                 110
    300                 250
    550                 380

(X) a) Cada par (x(i);y(i)) forma um exemplo do conjunto de dados de treinamento.
( ) b) Cada par (x(i);y(i)) é caracterizado pelo índice i que indica o número de variáveis
explanatórias do modelo de ML.
( ) c) Cada par (x(i);y(i)) forma os exemplos de teste referentes as duas variáveis explanatórias
x e y.
( ) d) De acordo com os índices i e j, em que x(i)
j , temos que x(2)
1 = 180.

3. Exercício 3 (Modelos de Regressão Linear Simples e Múltipla)
Se estamos diante de um problema de regressão linear múltipla com milhares de variáveis
explanatórias, qual recomendação abaixo é plausível para um cientista de dados que pretende
se debruçar sobre o problema?

( ) a) O cientista deve usar os métodos das equações normais ou decomposição de valores
singulares (SVD) para fazer o treinamento das milhares de variáveis explanatórias.
( ) b) O cientista de dados não deve utilizar a regressão linear para esse caso, uma vez
que não é possível para esse algoritmo fazer o treinamento de milhares de variáveis
explanatórias.
(X) c) O cientista de dados deve avaliar os algoritmos de aprendizagem do gradiente
descendente e suas derivações (e.g., gradiente descendente estocástico ou em minibatches),
pois o uso de equações normais ou técnicas como o SVD pode elevar a
complexidade de forma significativa para esse caso.
( ) d) O cientista de dados deve avaliar as soluções fechadas (analíticas) para o problema
como o uso das equações normais para reduzir a complexidade de processo de
treinamento.

4. Exercício 4 (Modelos de Regressão Linear Simples e Múltipla)
Sobre os conceitos relacionados com a equação mostrada abaixo, marque a alternativa
correta:

( ) a) J(q0;q1) consiste na função hipótese estimada que caracteriza o modelo de ML
( ) b) A diferença hq (x(i))􀀀y(i) é o principal parâmetro ajustável de um modelo de ML
( ) c) J(q0;q1) consiste na função custo utilizada no processo de treinamento e seu valor
(i.e., custo) não depende dos parâmetros q0 e q1.
(X) d) J(q0;q1) consiste na função custo utilizada no processo de treinamento e seu valor
(i.e., custo) depende dos parâmetros q0 e q1.

5. Exercício 5 (Algoritmo do Gradiente Descendente)
Marque a alternativa correta sobre o funcionamento do algoritmo do gradiente descendente

( ) a) O algoritmo do gradiente descendente é retratado pela atualização iterativa do
parâmetro aleatório a, denotado como taxa de aprendizagem.
( ) b) A atualização de cada parâmetro qj ocorre a partir de seu valor atual e do termo
que é formado pela taxa de variação (i.e., derivada) da função custo em relação à seus
parâmetros e o termo a.
( ) c) A atualização de cada parâmetro qj ocorre a partir de seu valor atual e do termo que
é formado pela taxa de variação (i.e., derivada) da função custo, que é constante a cada
iteração (loop) do algoritmo.
(X) d) A derivada parcial da função hipótese hx em relação ao parâmetro q é fundamental
para o algoritmo do gradiente, que é expressa pela tangente (i.e., inclinação) obtida
para o respectivo valor de q.

6. Exercício 6 (Modelos de Regressão Linear Simples e Múltipla)
Um cientista de dados inicia a fase de análise exploratória de um problema de regressão
e constata a diferença de escala, em termos de valores absolutos de diversas variáveis explanatórias
que poderão compor o modelo de ML a ser construído. Diante dessa situação,
marque a alternativa correta sobre duas questões: i) o impacto dessa diferença de valores
entre variáveis explanatórias no algoritmo de aprendizagem do gradiente descendente e ii)
qual seria a estratégia para lidar com esse problema?

( ) a) Sobre a questão i) o impacto direto da diferença de escala é visto na rapidez de
convergência do algoritmo do gradiente descendente, em razão do formato diferente
(mais circular) da função custo nesse caso e ii) uma estratégia consiste em aplicar o
dimensionamento de características por meio de técnicas de normalização para atribuir
uma escala equivalente aos dados, preservando suas características.
(X) b) Sobre a questão i) o impacto direto da diferença de escala é visto na demora de
convergência do algoritmo do gradiente descendente, em razão do formato diferente
(mais elíptico) da função custo nesse caso e ii) uma estratégia consiste em aplicar o
dimensionamento de características por meio de técnicas de normalização para atribuir
uma escala equivalente aos dados, preservando suas características.
( ) c) Sobre a questão i) não há impacto no algoritmo de aprendizagem do gradiente
descendente e ii) nesse sentido, o cientista pode seguir com o treinamento sem préprocessar
as variáveis explanatórias.
( ) d) Sobre a questão i) não existe um impacto no gradiente descendente, mas sim nas
equações normais que podem ser usadas no processo de aprendizagem ii) nesse caso, a
saída consiste em utilizar o gradiente descendente estocástico.

7. Exercício 7 (Álgebra matricial e equações normais)
O desenvolvimento abaixo mostra os procedimentos algébricos que resultaram no vetor
de parâmetros  sobre a solução das equações normais, em que X é a matriz de preditores
(variáveis explanatórias) e y é a variável de saída, i.e,

Baseado especificamente no cômputo final do estimador , marque a alternativa correta:
( ) a) O estimador  consiste em uma matriz singular.
( ) b) A estimação dos parâmetros depende de uma inversão matricial com complexidade
expressa por O(nlogn).
( ) c) As equações normais permitem fazer a estimação dos parâmetros se o determinante
do termo XTX for nulo.
(X) d) XTX é invertível se o seu determinante é diferente de zero.

8. Exercício 8 (Convergência do Algoritmo Gradiente Descendente)
Assumindo a função custo do erro quadrático médio referente ao problema de regressão
linear mostrada abaixo (trata-se de uma função convexa), marque a alternativa correta sobre
a convergência do algoritmo de aprendizagem gradiente descendente

( ) a) No caso citado, o algoritmo do gradiente descendente enfrentará problemas de
convergência, em razão dos diversos mínimos locais existentes na função custo do erro
quadrático médio.
(X) b) No caso citado, o algoritmo do gradiente descendente sempre alcançará o mínimo
global, em razão da característica convexa da função custo do erro quadrático médio,
ponderado pela inicialização dos parâmetros e o valor da taxa de aprendizagem a.
( ) c) No caso citado, o algoritmo do gradiente descendente enfrentará problemas de
convergência, em razão da característica convexão da função custo do erro quadrático.
( ) d) No caso citado, o algoritmo do gradiente descendente sempre alcançará o mínimo
local (que não é o mínimo global nesse caso), em razão da característica côncava da
função custo do erro quadrático médio, ponderado pela inicialização dos parâmetros e
o valor da taxa de aprendizagem a.

9. Exercício 9 (Normalização e o Algoritmo Gradiente Descendente)
Marque a alternativa correta sobre o funcionamento do algoritmo do gradiente descendente e
sua relação com a preparação e processamento dos dados.

( ) a) O valor dos parâmetros obtidos no processo de treinamento do modelo de regressão
não é influenciado pela normalização dos dados ou dimensionamento de características.
(X) b) A normalização realizada sobre os dados das variáveis explanatórias tem influência
sobre o valor dos parâmetros obtidos no processo de treinamento do modelo.
( ) c) A normalização dos dados ou dimensionamento de características não tem impacto
sobre a convergência do gradiente descendente.
( ) d) Se os dados foram normalizados o gradiente descendente funcionará normalmente e,
com isso, não é necessário procedimentos de normalização para a geração de predições
após o treinamento.

10. Exercício 10 (Interpretabilidade dos Modelos de Regressão Linear)
A Figura abaixo apresenta os resultados de treinamento de um modelo de regressão linear
simples conduzido na linguagem R. Sobre a interpretabilidade dos resultados obtidos,
marque a alternativa correta:

() a) O conhecimento estatístico sobre os testes de hipóteses e os níveis de significância
não podem ser aplicados sobre o resultado de treinamento, somente na fase de teste do
modelo de ML.
(X) b) A inspeção do o valor-p permite constatar a relação estatística entre um variável
explanatória e a saída ou resposta do modelo de ML.
() c) Os níveis de significância e seus códigos nos informam a relevância estatística da
variável de saída ou resposta para o modelo ML, auxiliando o cientista de dados na
geração de predições.
() d) Quanto menor os valor dos indicadores R-squared melhor é o poder explicativo do
modelo em relação aos dados.