# Objetivo Geral

Introdução ao versionameno de código com "<em>Git</em>" e "<em>GitHub</em>":

- Conhecer as ferramentas
- Instalar, Configurar e Autenticar
- Primeiros passos com Git e GitHub
- Dicas e materiais de apoio

## O que é "<em>Versionamento de Código</em>"

> ### <em>Sistemas de Controle de Versão (VCS)</em>:

Controlam as versões de um arquivo ao longo do tempo:

- Registra o histórico de atualizações de um arquivo
- Gerenciam quais foram as atualizações, as datas, autor, etc...
- Organização, Controle e Segurança

<br>

Dentre os Sistemas de Controle de Versão, temos:

> #### "<em>VCS Centralizado (CVCS)</em>":

Temos como Softwares:

- CVS, Subversion

Nele temos apenas um servidor que conterá todos os arquivos responsáveis por esse controle de versões, nisso, teremos as áreas de trabalhos conectadas ao servidor.

A sua desvantgem é que caso ele fique fora do ar, não é possível contribuir com versões, arquivos de código, ou caso algum arquivo esteja corrompido por alguma falha, todo o projeto poderá ser perdido.

<br>

> #### "<em>VCS Distribuído (DVCS)</em>":

Temos como Softwares:

- Git, Mercurial

Nele, o banco de versão é duplicado localmente e ambos teremos uma cópia dos arquivos que estarão ali naquele servidor localmente, permitindo editar os arquivos, mesmo que o servidor esteja fora do ar.

Algumas características dele é que ele clona o repositório completo, o que inclui o histórico de versões:

- Cada clone é como um backup
- Possibilita um fluxo de trabalho flexível
- Possibilidade de trabalhar sem conexão à rede

<br>

## O que é "<em>Git</em>"?

O Git é um "<em>Sistema de Controle de Versão Distribuído</em>"

- Gratuito e Open Source (Código Aberto)
- Ramificações (branching) e fusões (mergin) eficientes
- Leve e rápido

SCM → souce code management


> <a href="https://git-scm.com/">Saiba mais!</a>


### Breve histórico do Git:

- 2002: O projeto do "<em><b>núcleo (Kernel) do Linux</b></em>", que é open source, começa a utilizar o "<em><b>BitKeeper</b></em>", um "<em><b>DVCS proprietário</b></em>"

- 2005: Após alguns conflitos com a comunidade, o BitKeeper "<em>rescinde à licença gratuita</em>" o que leva à "<em>Linux Torvalds</em>",  o criador do Linux, e sua equipe à desenvolverem a sua própria ferramenta, o "<em>Git</em>".

<br>

-------


- Caso queiramos ter uma cópia do nosso repositório, precisamos digitar o comando "<code>git clone</code>" no terminal:

<code>
...\DIO\Engenharia_de_Dados_com_Python> git clone
</code>

<br>

- Então decidimos que queremos criar uma nova versão, e precisamos salvar... (Sempre no terminal) digitamos o comando "<code>git commit -m 'mensagem do que alteramos'</code>:"

<code>
...\DIO\Engenharia_de_Dados_com_Python> git commit -m 'mensagem'
</code>

<br>

- Para atualizar o repositório à partir do meu repositório remoto, utilizamos o comando "<code>git pull</code>", pois assim, "puxamos" qualquer alteração já feita antes por um colaborador:

<code>
...\DIO\Engenharia_de_Dados_com_Python> git pull
</code>

<br>

- E para enviar todas as alterações para o repositório remoto, utilizamos o comando "<code>git push</code>", pois assim, "empurramos" as alterações feitas por nós:

<code>
...\DIO\Engenharia_de_Dados_com_Python> git push
</code>
<br><br>

> ### Comandos:

- "<code>git clone</code>": clona um repositório Git existente para um novo diretório (pasta) Local.

- "<code>git commit</code>": grava alterações no repositório.

- "<code>git pull</code>": "puxa" as alterações do repositório remoto para o local (busca e mescla).

- "<code>git push</code>": "empurra" as alterações do repositório local para o repositório remoto.

<br>

## O que é GitHub?

Plataforma de hospedagem de código para controle de versão com Git, e colaboração.

- Comunidade ativa
- Utilizado mundialmente
- Mascote "<em>Octocat</em>"

### Breve histórico do Github:

- 2008: Desenvolvido por Chris Wanstrath, J. Hyett, Tom Preston-Werner e Scott Chacon.

- 2018: Vítima de um dos maiores "<em>ataques de DDoS</em>" (ataque distribuído de negação de serviço); Comprado pela "<em>Microsoft Corporation</em>" por "<em>$ 7,5 bilhões</em>".

O "<em>Git</em>" é a ferramenta que fará esse controle de versões, já o "<em>GitHub</em>" é a ferramenta que irá atuar como o servidor para a hospedagem dessas versões.