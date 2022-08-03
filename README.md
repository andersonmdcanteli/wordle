# Mastering WORDLE

## Intro

Inicialmente, precisamos de dados das palavras que podem ser utilizadas no jogo. O jogo conta com dois conjuntos dados: o que contém apenas as respostas possíveis; o que contém todas as palavras aceitas com excessão das possíveis respostas. Assim, temos 3 datasets:

Dataset 1: contém apenas as palavras que podem ser a palavra do dia

Dataset 2: contém apenas as palavras aceitas, desconsiderando as palavras que podem ser a palavra do dia

Dataset 3: contém todas as palavras aceitas (combinação do Dataset 1 e Dataset 2).

Como desejamos saber qual é o melhor chute para o primeiro chute e para o primeiro par de chutes, é importante verificar a relação entre estes conjuntos.



Assim, existem diferenças entre os datasets, porém elas não são significativas. Contudo, como o dataset 3 é mais completo, ele é melhor.

A seguir seguem os resultados obtidos para cada dataset. Cada dataset tem 3 resultados distintos, que variam em relação a forma de estimar a força das palavras. De forma resumida:

Forma 1: considera a frequência das letras em relação a todas as letras do dataset

Forma 2: considera a frequência das letras em relação a todas as letras do dataset, penalizando as palavras que tem letras repetidas

Forma 3: considera a frequência das letras em relação a todas as letras do dataset, penalizando as palavras que tem letras repetidas e considera a posição das letras nas palavras.


## Results for Dataset 1

### Considering only the frequency of the letters in each word

#### First guess

##### Best 10 words

##### Worst 10 words


#### First two guesses

##### Best 10 words

##### Worst 10 words


### Adding penalty to words with repeated letters

#### First guess

##### Best 10 words

##### Worst 10 words


#### First two guesses

##### Best 10 words

##### Worst 10 words



### Adding the frequency of letters at each word position

#### First guess

##### Best 10 words

##### Worst 10 words


#### First two guesses

##### Best 10 words

##### Worst 10 words




## Results for Dataset 2

### Considering only the frequency of the letters in each word

#### First guess

##### Best 10 words

##### Worst 10 words


#### First two guesses

##### Best 10 words

| Word 1 | Word 2 | Rank |
| :-: | :-: | :-: |
| esses	| sessa	| 1 |
| asses	| esses	| 1 |
| esses	| sasse	| 1 |
| asses	| sasse	| 2 |
| asses	| sessa | 2 |
| sasse	| sessa	| 2 |
| esses	| sease | 3 |
| eases	| esses	| 3 |
| sease	| sessa	| 4 |
| sasse	| sease	| 4 |
| asses	| eases	| 4 |
| eases	| sasse	| 4 |
| asses	| sease	| 4 |
| eases	| sessa	| 4 |
| eases	| sease	| 5 |
| esses	| sises	| 6 |
| esses	| oases	| 7 |
| esses	| reses	| 8 |
| esses	| seers	| 8 |
| erses	| esses	| 8 |
| esses	| seres	| 8 |
| asses	| sises	| 9 |
| sasse	| sises	| 9 |
| sessa	| sises	| 9 |
| esses	| seise	| 10 |



##### Worst 10 words


### Adding penalty to words with repeated letters

#### First guess

##### Best 10 words

##### Worst 10 words


#### First two guesses

##### Best 10 words

##### Worst 10 words



### Adding the frequency of letters at each word position

#### First guess

##### Best 10 words

##### Worst 10 words


#### First two guesses

##### Best 10 words

##### Worst 10 words




