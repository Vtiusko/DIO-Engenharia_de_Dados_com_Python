# Configurações no Git

O comando "<em>git config</em>" permite visualizar e definir variáveis de configurações do nosso git. Essas variáveis ficam armazenadas especialmente em três lugares:

- git <code>--global</code>: referente as configurações no usuário
- git <code>--system</code>: referente as configurações no sistema como um todo, que abriga todos os usuários
- git <code>--local</code>: referente à configuração de um repositório específico, no qual nos encontramos.

<br>

- Vamos Configurar nome de usuário e e-mail para podermos utilizar o Git e GitHub:
    - No "<em>Git Bash</em>", vamos digitar o comando "<em>git --global user.name (nome de usuário)</em>": 
    <br>
    > <code>git --global user.name 'nome de usuário'</code>
    
    <br>
    
    - Logo após, vamos utilizar o comando "<em>git --global user.email (endereço de e-mail)</em>":
    <br>
    > <code>git --global user.em    ail endereço_de_e-mail</code>

    <br>

    - E para verificar quais alterações foram feitas, podemos utilizar o comando:
        - "<em>git config user.name</em>" → Para o usuário
        - "<em>git config user.email</em>" → Para o e-mail

    <br>

    - Para renomear-mos o nome da nomssa Branch, de "<em>master</em>" para "<em>main</em>", primeiro utilizamos o comando "<em>git config init.defaultBranch</em>" para verificar o nome da nossa "<em>Branch</em>":
    
    > <code>git config init.defaultBranch</code>

    <br>

    e então o comando para alterar de master para main, no "<em> --global</em>":

    > <code>git config --global init.defaultBranch main</code>

<br><br>