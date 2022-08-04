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

### First guess

Source: [notebook](https://github.com/andersonmdcanteli/wordle/blob/main/wordle_only_answers_first_guess.ipynb).

#### Best 10 words

| Word | Rank |
| :-: | :-: |
| slate	| 1 |
| crane	| 2 |
| stare	| 3 |
| share	| 4 |
| crate	| 5 |
| snare	| 6 |
| trace	| 7 |
| saute	| 8 |
| stale	| 9 |
| shale	| 10 |



#### Worst 10 words

| Word | Rank |
| :-: | :-: |
| mimic	| 2303 |
| vivid	| 2304 |
| mamma	| 2305 |
| mucus	| 2306 |
| lymph	| 2307 |
| humph	| 2308 |
| fluff	| 2309 |
| jumbo	| 2310 |
| humus	| 2311 |
| nymph | 2312 |




### First two guesses

Source: [notebook](https://github.com/andersonmdcanteli/wordle/blob/main/wordle_only_answers_pair_of_words.ipynb).

#### Best 10 words

| Word 1 | Word 2 | Rank |
| :-: | :-: | :-: |
| crony	| slate	| 1 |
| soapy	| trice	| 2 |
| crone	| shalt	| 3 |
| price	| slant	| 4 |
| briny	| slate	| 5 |
| crime	| slant	| 6 |
| grant	| slice	| 7 |
| crone	| salty	| 8 |
| corny	| slate	| 9 |
| brine	| soapy	| 10 |


#### Worst 10 words


| Word 1 | Word 2 | Rank |
| :-: | :-: | :-: |
| rumba	| umbra	| 526085 |
| ennui	| undid	| 526086 |
| humus	| mummy	| 526087 |
| mucus	| music	| 526088 |
| fluff	| lupus	| 526089 |
| lupus	| usurp	| 526090 |
| humph	| thump	| 526091 |
| chump	| humph	| 526092 |
| humus	| mucus	| 526093 |
| humph	| humus	| 526094 |






## Results for Dataset 2



### First guess

Source: [notebook](https://github.com/andersonmdcanteli/wordle/blob/main/wordle_only_allowed_first_guess.ipynb).

#### Best 10 words

| Word | Rank | &nbsp; | Word\* | Rank\* | 
| :-: | :-: | :-: | :-: | :-: |
| tares	| 1	| &nbsp; | soare | 1 |
| lares	| 2	| &nbsp; | saine | 2 |
| pares	| 3	| &nbsp; | slane | 3 |
| dares	| 4	| &nbsp; | saice | 4 |
| cares	| 5	| &nbsp; | soave | 5 |
| bares	| 6	| &nbsp; | saree | 6 |
| mares	| 7	| &nbsp; | slade | 7 |
| gares	| 8	| &nbsp; | sarge | 8 |
| nares	| 9	| &nbsp; | prase | 9 |
| hares	| 10	| &nbsp; | coate | 10 |

\* estimated with the frequencies obtained using dataset 1



#### Worst 10 words


| Word | Rank | &nbsp; | Word\* | Rank\* | 
| :-: | :-: | :-: | :-: | :-: |
| chuff | 10538 | &nbsp; | hypha | 10432 |
| uhuru	| 10539	| &nbsp; | gyppo | 10433 |
| enzym	| 10540	| &nbsp; | kibbi | 10434 |
| gyppy	| 10541	| &nbsp; | kudzu | 10435 |
| phpht	| 10542	| &nbsp; | immix | 10436 |
| immix	| 10543	| &nbsp; | fuffs | 10437 |
| xylyl	| 10544	| &nbsp; | kukus | 10438 |
| hyphy	| 10545	| &nbsp; | jujus | 10439 |
| undug	| 10546	| &nbsp; | imshi | 10440 |
| ungum	| 10547	| &nbsp; | umphs | 10441 |

\* estimated with the frequencies obtained using dataset 1



### First two guesses

#### Best 10 words


##### Worst 10 words



## Results for Dataset 3



### First guess

#### Best 10 words

#### Worst 10 words


### First two guesses

#### Best 10 words


##### Worst 10 words








