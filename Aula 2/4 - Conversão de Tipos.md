# Objetivo Geral
- Aprender a converter os tipos das variáveis

<br>

## Convertendo Tipos

Em alguns momentos é necessário (ou será necessário) converter o tipo de uma variável para manipular seu conteúdo de forma diferente. Por exemplo:

- Variáveis do tipo "<em>string</em>", que armazenam números e precisamos fazer alguma operação matemática com esse valor.

<br>

<code>
numero_string = '10'<br>
num_convertido_para_int = int(numero_string)<br><br>
print(type(num_convertido_para_int))<br><br>
Saída: < class 'int' >
</code>

<br>

## Erro de Conversão

Nem sempre vai dar para converter um tipo para outro, por exemplo, de "<em>string</em>" para um valor "<em>numérico</em>", esse tipo de conversão nos é gerado um "<em>ValueError</em>":

<br>

<code>
preco = 'python'<br>
print(float(preco))<br><br>
>>><br>
Traceback (most recent call last):<br>
| File 'nome_do_arquivo'.py, line 3, in < module ><br>
| print(float(preco))<br>
ValueError: could not convert string to float: 'python'
</code>

<br>

