# Objetivos Gerais

- Entender o que são e como utilizar "<em>Variáveis</em>" e "<em>Constantes</em>".

<br>

## O que são "<em>Variáveis</em>" e "<em>Constantes</em>"

Em linguagens de programação podemos definir valores que podem sofrer alterações no decorrer da execução do programa. Esses valores recebem o nome de "<em>variáveis</em>", pois elas nascem com um valor e não necessáriamente devem permanecer com o mesmo durante a execução do programa.

<br>

<code>
Podemos fazer em formar de "<em>Unpacking</em>":<br><br>
> nome, idade = 'Victor Guilherme', 24<br><br>
--------------------------------------------------------<br>
Como podemos definir linha por linha:<br><br>
> nome = 'Victor Guilherme'<br>
> idade = 24<br><br><br>
print(f'Olá, meu nome é {nome}, eu tenho {idade} anos')
</code>

<br>

## Alterando os valores

No python, não precisamos definir o tipo de dados da variável (como no Java por exemplo), o interpretador do Python faz isso automaticamente para nós. Por isso "<em>não podemos simplesmente criar uma variável sem atribuir um valor</em>". Para alterar o valor de uma variável, basta fazer uma atribuição de um novo valor:

<br>

<code>
idade = 25<br><br>
print(f'Na verdade, eu tenho {idade} anos')
</code>

<br>

## Constantes
Assim como as variáveis, constantes são utilizadas para armazenar valores. Uma constante nasce com um valor e permanece com ele até o final da execução do programa, ou seja, o valor é imutável.

<br>

## Python não tem Constantes

Não existe uma palavra reservada para informar ao interpretador que o valor é uma constante. Em algumas linguagens por exemplo: Java e C utilizamos "<em>final</em>" e "<em>const</em>", respectivamente para declarar uma constante.

Em python, usamos a "<em>convenção</em>" que diz ao programador que a variável é uma constante. Para fazer isso é necessário criar a variável toda em letra "<em>Maiúsculas</em>". Alguns exemplos de constantes:

<br>

<code>
ABS_PATH = ...\DIO\Engenharia_de_Dados_com_Python\Aula 2...<br><br>
DEBUG = True<br><br>
ESTADOS = [<br>
|   SP,<br>
|   MG,<br>
|   SP,<br>
|   ...<br>
]
</code>

<br>

## Boas Práticas
- O padrão de nomes devem ser em "<em>snake case</em>" - (total_compra, valor_final...)
- Escolher nomes sugestivos
- Nomes de constantes todo em maiúsculo