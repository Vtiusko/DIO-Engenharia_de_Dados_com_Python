# Objetivo Geral

    Conhecer os tipos de dados mais utilizados no Python.

<br>

## O que são tipos?

    Os tipos servem para definir as características e comportamento de um valor (objeto) para o interpretador. Por exemplo:

<em>
'''
Esse tipo eu sou capaz de realizar operações matemáticas...<br>
Esse tipo para ser armazenado em memória irá consumir 24 bytes...'''
</em>

<br>

## Tipos em Python

    Os tipos de dados em Python são (os mais comuns, aqui não estão todos):

>   - STR → cadeia de carácteres (tudo entre aspas simples ou duplas é um texto).
>   - INT, FLOAT, COMPLEX → são os 3 tipos númericos no python.
>   - LIST, TUPLE, RANGE → são uma sequência (lista, tupla e conjunto).
>   - DICT → um mapa com valores "chave" : "valor". 
>   - SET, FROZENSET → são uma coleção.
>   - BOOL → valores booleanos (True ou False).
>   - BYTES, BYTEARRAY, MEMORYVIEW → são tipos binários no python.

<br>

## Tipos Numéricos

### Inteiros (INT):

Números inteiros são representados pela classe "<em>int()</em>" e possuem precisão ilimitada. São exemplos válidos de números inteiros valores como:

>   1, 10, 100, -659, 95, ... 166525612560125541...

<br>

### Ponto Flutuante (FLOAT):

Os números de ponto flutuante são usados para representar os números racionais (com casas decimais) e sua implementação é feita pela classe "<em>float()</em>". São exemplos válidos de números de ponto flutuante valores como:

>   1.5, 10.9, 100.0012, -695.6168161, ...

<br>

### Booleanos (BOOL):

É usado para representar "<em>Verdadeiro</em>" ou "<em>Falso</em>", e é implementado pela classe "<em>bool()</em>". Em Python o tipo booleano é uma subclasse de "<em>int</em>", uma vez que qualquer número diferente de 0 representa "<em>True</em>", e 0 representa sempre "<em>Falso</em>". Exemplos válidos de valores booleanos:

>   True e False

<br>

### Strings - Cadeia de Cadeia de Carácteres (STR):

"<em>Strings</em>" ou "<em>Cadeia de Carácteres</em>" são usadas para representar "<em>Valores Alfanuméricos</em>", esses valores devem estar entre aspas simples '' ou duplas "", não importa qual você vai utilizar, desde que a mesma aspa seja utilizada para "fechar" a string. Em Python as strings são definidas pela classe "<em>str()</em>". São exemplos válidos de strings:

>   "Python", 'Python', "1235_@#$%", '4868E=unasç'