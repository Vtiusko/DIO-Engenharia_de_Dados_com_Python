# Objetivo Geral

- Aprender como receber e exibir informações para o usuário

<br>

## Lendo valores com a função "<em>Input</em>"

A função "<em>builtin Input</em>" é utilizada quando queremos ler dados de entrada padrão (pelo teclado). Ela recebe um argumento do tipo "<em>string</em>", que é exibido para o usuário na saída padrão (tela). A função lê a entrada, converte para string e retorna o valor.

<br>

<code>
nome = input('Digite seu nome: ')<br>
>>> Digite seu nome: 
</code>

<br>

## Exibindo os valores com a função "<em>Print</em>"

A função "<em>builtin Print</em>" é utilizada quando queremos exibir dados na saída padrão (tela). Ela recebe um argumento obrigatório do tipo "<em>varargs</em>" de objetos e 4 argumentos opcionais:

- sep
- end
- file
- flush

Todos os objetos são "<em>convertidos</em>" para string, "<em>separados</em>" por sep e "<em>terminados</em>" por end. A string final é exibida para o usuário.

<br>

<code>
nome = 'Victor'<br>
sobrenome = 'Guilherme'<br><br>
print(nome, sobrenome)<br>
print(nome, sobrenome, end='...\n')<br>
print(nome, sobrenome, sep='#')<br><br>
Saídas:<br>
Victor Guilherme<br>
Victor Guilherme...<br>
Victor#Guilherme
</code>