# Algoritmos de aprendizado de máquina supervisionado com Python

## Aprendizado supervisionado
- Um conjunto de variáveis independentes é utilizado para predizer uma variável dependente. Os valores da variável dependente são conhecidos.
- Exemplo: predizer a idade de pessoas com base na altura e peso
- Variáveis independentes: altura e peso
- Variável dependente: idade 

## Os seguintes algoritmos serão estudados e testados
- Regressão logística
- KNN 
- Naive Bayes
- SVM
- Árvores de decisão

### Regressão logística
- A regressão logística é uma técnica que nos permite estimar a probabilidade associada à ocorrência de determinado evento dado um conjunto de variáveis independentes.
- A função tem forma de S e varia entre 0 e 1.
- Variável dependente categórica. Exemplos:
  - Predizer se um email é spam (1) ou não (0)
  - Predizer se um tumor é maligno (1) ou não (0)
  
![myImage](https://www.analyticsvidhya.com/wp-content/uploads/2015/11/plot.png)

### KNN
- É um algoritmo de classificação em que a classe de uma nova observação é definida com base nas K observações vizinhas.
- É um algoritmo “preguiçoso”, que não precisa de dados de treinamento.
- Passo do algoritmo:
  - Calcular distância 
  - Encontrar os pontos/vizinhos mais próximos
  - Votar a label para o ponto a ser previsto

![myImage](https://d3b8hk1o42ev08.cloudfront.net/wp-content/uploads/res.cloudinary.com/dyd911kmh/image/upload/f_autoq_autobest/v1531424125/KNN_final1_ibdm8a.png)

### Naive Bayes
- O algoritmo recebe o nome de “naive” (ingênuo) porque desconsidera a correlação entre as variáveis (features).
- É um classificador probabilístico baseado no Teorema de Bayes.
- Conhecimentos prévios dos dados guiam decisões de classificação.

![myImage](https://www.analyticsvidhya.com/wp-content/uploads/2015/09/Bayes_rule-300x172-300x172.png)

### SVM
- O objetivo do SVM (Máquina de Vetores de Suporte) é encontrar um hiperplano em um espaço N-dimensional (N é o número de variáveis) que maximiza a distância entre dados de diferentes classes.
- Maximizar a margem de distância fornece mais segurança de que novas observações serão classificadas com mais confiança.

![myImage](https://www.saedsayad.com/images/SVM_2.png)
