# Algoritmos de aprendizado de máquina não supervisionados com Python

## Aprendizado não supervisionado
- Um conjunto de variáveis é classificado em grupos com base na similaridade entre elas
- O conjunto de dados não possui uma variável dependente

## Motivação
- Nem sempre temos dados com labels/alvos definidos
  - Pela natureza da fenomenologia
  - Pelo custo de se produzir esse tipo de dados
- Problemas que não são de classificação ou regressão
  - Entender tipos de clientes que uma determinada empresa possui
  - Estimativa da distribuição de dados
  - Categorização, sem categorias pré-definidas

## Algoritmos que podem ser utilizados
- K-means
- Mapa de Kohonen
- Rede ART

### K-means
- K observações dentro do conjunto de dados são escolhidas aleatoriamente como centróides iniciais
- K clusters são criados, associando cada observação ao centróide mais próximo (mais similar)
- Na etapa de atualização, o centróide de cada um dos K cluster se torna a nova média entre as entradas associadas à cada cluster
- Estes passos são repetidos até a convergência, isto é, quando as entradas não trocam de clusters

![myImage](https://i.imgur.com/k4XcapI.gif)

### Mapa de Kohonen
- Escolhe-se o número de neurônios inicial
  - A inicialização do centro de cada cluster pode ser aleatória ou pode partir do próprio conjunto de entradas
- Cada entrada é atribuída ao neurônio (cluster) mais próximo (similar)

![myImage](https://upload.wikimedia.org/wikipedia/commons/thumb/3/35/TrainSOM.gif/220px-TrainSOM.gif)

### Rede ART (Adaptive Resonance Theory)
- O principal parâmetro é o raio de similaridade mínima r0
- A primeira entrada apresentada à rede é considerada como um neurônio
- A segunda entrada é comparada com o neurônio já existente e com r0
  - Se esta entrada for similar ao neurônio já existente, ela atualiza os pesos do mesmo
  - Caso contrário, um novo neurônio é criado
  
_Observações_
 - Não é preciso definir um número inicial de cluster
 - A definição do raio de similaridade mínima pode ser complicada
 - Custo de treinamento é elevado
    - Regra delta, essencialmente sequencial
    - Algumas maneiras de otimizar o processo

![myImage](https://www.tutorialspoint.com/artificial_neural_network/images/supplement_unit.jpg)
