# O que é O ".md" ou arquivo "MarkDown"?

Markdown é "<em>uma linguagem de marcação simples</em>", seria uma forma mais simples de estar escrevendo o "<em>HTML</em>", mas comparado ao Markdown, é um pouco mais complexa.

<br>

📖 Documentações:

- 🔷 [Documentação GitHub]("https://docs.github.com/pt/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/quickstart-for-writing-on-github")
- 🔷 [Documentação Git]("https://git-scm.com/doc")

<br>

## Criando e Clonando Repositórios

> Existem duas formas de se obter um repositório Git na minha máquina:

- Transformando um "<em>Repositório Local</em>" que não está sob controle de versão, num "<em>Repositório Git</em>".

- "<em>Clonando</em>" um repositório Git existente.

<br>

> ## Passo à Passo:

<b><em>ATALHOS</em></b>:

> • <b>Ctrl + L</b> = comando que limpa o terminal<br>
> • <b>ls</b> = comando que retorna todo os arquivos dentro de uma pasta<br>
> • <b>cat</b> = comando que exibe todo o conteúdo de um arquivo<br>
> • <b>cd ..</b> = comando que retorna para o diretório anterior<br>
> • <b>touch nome_do_arquivo</b> = comando que cria um arquivo com o nome desejado 

<br>

- 1º Forma: Criar uma pasta que desejamos transformar num repositório Git:
    - No "<em>Git Bash</em>", vamos digitar o comando "<em>mkdir (nome da pasta)</em>":<br><br>

    > <code>mkdir nome_da_pasta</code>
    
    <br>

    - Logo após, vamos entrar na pasta que criamos, utilizando o comando "<em>cd (nome da pasta)</em>":<br><br>

    > <code>cd nome_da_pasta_que_criamos</code>

    <br>

    - Dentro dessa pasta, vamos digitar o comando "<em>git init</em>", assim ele será transformado num repositório Git:<br><br>
    
    > <code>git init</code>

    <br>

    "<em>Origin</em>" é o nome padrão que o Git dá ao servidor que clonamos o repositório, além de passar a "<em>URL</em>" desse repositório na hora do clone.

    Quando transformamos um repositório Local em um repositório Git, é crucial que vinculemos ele à um repositório remoto. Para confirmar se ele está ou não vínculado à um repositório remoto, podemos utilizar o comando "<em>git remote -v</em>", onde ele mostra todos os repositórios remotos que eu estou vínculado:<br><br>

    > <code>git remote -v</code>

    <br>

    Para conectarmos esse repositório Local ao repositório Remoto, vamos utilizar o comando "<em>git remote add origin (ou o nome que eu quiser dar pra ele no lugar de origin) url_do_repositorio_no_github</em>":<br><br>
    
    > <code>git remote add origin url_desse_repositorio_no_github</code>

<br><br>

- 2º Forma: Clonar um repositório Git à prtir da url:<br>

    • No "<em>GitHub</em>", vamos entrar no nosso repositório, e no botão "<em>code</em>", vamos clicar e depois clicar na opção "<em>HTTPS</em>" e vamos copiar o link que aparece.

    <br>

    • Logo após, vamos entrar na pasta que criamos, utilizando o comando "<em>cd (nome da pasta)</em>":
    <br><br>

    > <code>cd nome_da_pasta_que_criamos</code>

    <br>

    • Dentro dessa pasta, vamos digitar colar a url que copiamos junto com o comando "<em>git clone 'url que copiamos'</em>", assim ele irá clonar um repositório Git para o repositório Local:
    <br><br>

    > <code>git clone 'url que foi copiada'</code>

    <br>

    Caso queiramos que no nosso computador esse repositório seja de um outro nome, sem ser do que está no GitHub, podemos redefini-lo apenas passando o nome dele como último argumento:<br><br>

    > <code>git clone 'url que foi copiada' novo_nome</code>
       
<br><br>

----

<br><br>

# Salvando Alterações no Repositório Local

Vamos criar um repositório com a finalidade de organizar os resumos das aulas (muito prático para poder treinar com Git e GitHub)!

- Vamos analisar um pouco mais a respeito do comando "<em>git status</em>", como o nome já diz, é responsável por mostrar a nossa "<em>árvore de trabalho</em>" e "<em>área de prepraração</em>", que é onde estaremos preparando os nossos arquivos, para serem "empacotados" num commit:<br><br>
    
    > <code>git status</code>

    <br>

Se houverem arquivos que não foram "comitados", o git status irá nos retornar um "<em>Untracked Files</em>" que significa "<em>Arquivos não Rastreados</em>", são arquivos que o git desconhece, ou seja, estão presentes aqui na área de trabalho, porém não estavam presentes na área de preparação e em nenhum commit anterior.

<br>

Logo após ter realizada todas as alterações no nosso arquivo, vamos executar o comando "<em>git add</em>". Porém através do git add, podemos ou "<em>adicionar apenas 1 arquivo</em>" ou, "<em>podemos adicionar todos os arquivos de uma vez</em>" para a área de preparação.

- Para adicionar apenas um arquivo em específico:<br><br>

    > <code>git add nome_do_arquivo</code>

    <br>

- Para adicionar TODOS os arquivos, para isso utilizamos o ponto ( . ):<br><br>

    > <code>git add .</code>

<br>

Após, podemos conferir com o comanado git status novamente como estão nossos arquivos, e no git bash já vai estar mostrando que há arquivos prontos para serem "comitados", assim podemos utilizar o comando "<em>git commit -m 'mensagem de commit'</em> ".<br><br>

> <code>git commit -m 'mensagem do commit'</code>

<br>

Se digitarmos o comando "<em>git log</em>" podemos estar visualizando o commit que acabamos de fazer, além de mostrar o autor, hash("identidade do commit"), data e endereço de e-mail:<br><br>

> <code>git log</code>

<br>

O Git não reconhece pastas de diretórios vazios, para que ele reconheça é necessário que seja adicionado algum arquivo dentro dele.<br>

Algumas vezes vamos preferir que o Git "não veja" nossos arquivos, para isso devemos informar dentro do aqruivo "<em>.git ignore</em>" o nome de nossas extensões, nome do arquivo, ou até mesmo trachos iniciais deles, pois assim eles serão ignorados pelo git, e ficarão apenas em nosso computador!<br>

- Vamos executar o comando "<em>echo</em>" e informar o nome do nosso diretório, arquivo ou extensão que queremos que o git não leve em consideração. Se for um diretório, devemos passar "nome do diretório e /"<br><br>

    > <code>echo nome_do_que_vai_ser_ignorado > .gitignore</code>

<br>

- Para fazer com que o git possa considerar novamente o nosso diretório, arquivo ou extensão vamos executar o comando "<em>echo > .gitignore</em>".<br><br>

    > <code>echo > .gitignore</code>

<br>

É bem comum que quando formos verificar outros repositórios, encontrarmos arquivos como "<em>.gitkeep</em>" dentro dos diretórios. Esse arquivo nada mais é do que uma convenção para que o Git reconheça diretórios vazios.

Na aula a professora utilizou o comando: "<code>touch aulas/.gitkeep</code>" (que funciona para sistemas operacionais Linux e MacOS), porém omo estou no Windowns, o comando que funcionou pra mim foi: "<code>type NUL > aulas/.gitkeep</code>"

- Esse comando cria um arquivo vazio chamado .gitkeep dentro da pasta "aulas".<br>

> ### Por que criar um arquivo <b>.gitkeep</b>?<br>
> 
> <em>O arquivo .gitkeep é um arquivo vazio que serve para indicar ao Git que uma pasta deve ser rastreada, mesmo que ela não contenha outros arquivos. Isso é útil para manter pastas vazias sob controle de versão.</em>

<br>

----------