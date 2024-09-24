# Objetivo Geral

- Como usar o "<em>Modo Interativo</em>" do interpretador Python.
- Funções "<em>dir</em>" e "<em>help</em>"

<br>

## O "<em>Modo Interativo</em>"

O interpretador Python pode executar o código em modo que possibilite o desenvolvedor à escrever o código, e ver o resultado na hora.

Existem duas formas de iniciar o modo interativo:

- Chamando apenas no interpretador no terminal: <code>python</code>
- Executando o script(arquivo) com a flag -i: <code>python -i "nome 
_do_arquivo".py</code>.

<br>

>   Para sair do interpretador é necessário digitar:
-   <code>exit()</code>

<br>

## Funções "<em>dir</em>" e "<em>help</em>"
### dir:

Sem argumentos, retorna a lista de nomes no escopo local atual.
- dir → Mostra todos os aquivos/escopos do diretório atual

<code>
...\DIO\Engenharia_de_Dados_com_Python> dir<br><br>Diretório: C:\Users\victo\OneDrive\Área de Trabalho\Projetos\Cursos\DIO\Engenharia_de_Dados_com_Python<br><br>
Mode                 LastWriteTime         Length Name<br>
d-----        14/09/2024     13:20                Aula 1<br>
d-----        14/09/2024     14:21                Aula 2
</code>

<br>

Se eu chamar <code>python</code> no terminal:

<code>
...\DIO\Engenharia_de_Dados_com_Python> python<br>
Python 3.11.9 (tags/v3.11.9:de54cf5, Apr  2 2024, 10:12:12) [MSC v.1938 64 bit (AMD64)] on win32<br>
Type "help", "copyright", "credits" or "license" for more information.
</code>

<br>

E em seguida chamar a função dir(), nos é retornado o escopo:

<code>
>>> dir()<br>
['__annotations__', '__builtins__', '__doc__', '__loader__', '__name__', '__package__', '__spec__']
</code>

<br><br>



Com um argumento, retorna uma lista de atributos válidos para o objeto.

- dir(100):

<code>
>>> dir(100)<br>
['__abs__', '__add__', '__and__', '__bool__', '__ceil__', '__class__', '__delattr__', '__dir__', '__divmod__', '__doc__', '__eq__', '__float__', '__floor__', '__floordiv__', '__format__', '__ge__', '__getattribute__', '__getnewargs__', '__getstate__', '__gt__', '__hash__', '__index__', '__init__', '__init_subclass__', '__int__', '__invert__', '__le__', '__lshift__', '__lt__', '__mod__', '__mul__', '__ne__', '__neg__', '__new__', '__or__', '__pos__', '__pow__', '__radd__', '__rand__', '__rdivmod__', '__reduce__', '__reduce_ex__', '__repr__', '__rfloordiv__', '__rlshift__', '__rmod__', '__rmul__', '__ror__', '__round__', '__rpow__', '__rrshift__', '__rshift__', '__rsub__', '__rtruediv__', '__rxor__', '__setattr__', '__sizeof__', '__str__', '__sub__', '__subclasshook__', '__truediv__', '__trunc__', '__xor__', 'as_integer_ratio', 'bit_count', 'bit_length', 'conjugate', 'denominator', 'from_bytes', 'imag', 'numerator', 'real', 'to_bytes']
</code>

<br>

Em outras palavras, o que eu passar como parâmetro para a fução "<em>dir</em>", ele irá retornar todos os métodos e funções do parâmetro que eu passei!

<br>

### help:
Invoca o sistema de ajuda integrado. è possível fazer buscas em modo interativo (lembrando que para entrar no modo interativo é necessário digitar no terminal <code>python</code>):

<code>
PS C:\Users\victo\OneDrive\Área de Trabalho\Projetos\Cursos\DIO\Engenharia_de_Dados_com_Python> python<br><br>
Python 3.11.9 (tags/v3.11.9:de54cf5, Apr  2 2024, 10:12:12) [MSC v.1938 64 bit (AMD64)] on win32<br><br>
Type "help", "copyright", "credits" or "license" for more information.<br>
>>> help()
</code>

<br>

Após aparecerá uma mensagem, onde nele poderemos digitar qualquer coisa que queremos saber no python:

<code>
Welcome to Python 3.11's help utility! If this is your first time using
Python, you should definitely check out the tutorial at
https://docs.python.org/3.11/tutorial/.<br><br>

Enter the name of any module, keyword, or topic to get help on writing
Python programs and using Python modules.  To get a list of available
modules, keywords, symbols, or topics, enter "modules", "keywords",
"symbols", or "topics".

Each module also comes with a one-line summary of what it does; to list
the modules whose name or summary contain a given string such as "spam",
enter "modules spam".

To quit this help utility and return to the interpreter,
enter "q" or "quit".

help> "aqui digitamos o que queremos saber"
</code>

Pra sair basta digitar "<code>q</code>" e depois"<code>quit()</code>".

<br>

Ou podemos informar por parâmetro diretamente o nome do módulo, função, classe, método ou variável:

<code>
PS C:\Users\victo\OneDrive\Área de Trabalho\Projetos\Cursos\DIO\Engenharia_de_Dados_com_Python> python<br><br>
Python 3.11.9 (tags/v3.11.9:de54cf5, Apr  2 2024, 10:12:12) [MSC v.1938 64 bit (AMD64)] on win32<br><br>
Type "help", "copyright", "credits" or "license" for more information.<br>
>>> help(float)
</code>

<br>

E nos retorna-rá:

<code>
Help on class float in module builtins:
<br><br>
class float(object)<br>
 |  float(x=0, /)<br>
 |<br>
 |  Convert a string or number to a floating point number, if possible.<br>
 |<br>
 |  Methods defined here:<br>
 |<br>
 |  __abs__(self, /)<br>
 |      abs(self)<br>
 |<br>
 |  __add__(self, value, /)<br>
 |      Return self+value.<br>
 |<br>
 |  __bool__(self, /)<br>
</code>