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
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |




asses	esses	1.074862	1
esses	sasse	1.074862	1
asses	sasse	1.067017	2
asses	sessa	1.067017	2
sasse	sessa	1.067017	2
esses	sease	1.064221	3
eases	esses	1.064221	3
sease	sessa	1.056376	4
sasse	sease	1.056376	4
asses	eases	1.056376	4
eases	sasse	1.056376	4
asses	sease	1.056376	4
eases	sessa	1.056376	4
eases	sease	1.045735	5
esses	sises	1.038773	6
esses	oases	1.031472	7
esses	reses	1.031341	8
esses	seers	1.031341	8
erses	esses	1.031341	8
esses	seres	1.031341	8
asses	sises	1.030928	9
sasse	sises	1.030928	9
sessa	sises	1.030928	9
esses	seise	1.028132	10





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




