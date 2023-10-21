# 📝Módulo 3⇒ Git e GitHub

---

## Aula X ⇒

---

**AULA 1- Visão geral do Curso e Ferramentas**

**Passos do curso⇒**

- Conhecer as ferramentas;
- Instalar, configurar e autenticar;
- Primeiros passos com Git e GitHub;
- Dicas e materiais de apoio:

**O que é versionamento de código?**

— São as mudanças da versão de um código de forma contínua

**O que são Sistemas de controle de versão?**

—São sistemas que auxiliam a administrar versões de determinado código para que não fique algo desorganizado e confuso para equipe que está trabalhando nesse código

**Tipos de sistemas de Controle⇒**

**CVCS⇒**

Controle de versão centralizado, nele, as informações vão estar alocadas em um server principal, e se, por algum motivo, houver a rompimento de algum arquivo e não tiver um backup adequado, então esse arquivo será perdido>

**DVCS⇒**

Pensando nos problemas do controle de versão centralizado, foi criado o controle de versão distribuído, que cria cópias dos arquivos para cada indivíduo e da mesma forma aloca eles no server principal. 

- Nele, é possível ter um fluxo de trabalho flexível;
- É possível trabalhar nele sem conexão a rede:

**O que é Git?**

- É um sistema de controle de versão distribuído;
- Open source;
- Ramificações(branching) e fusões (merging) eficientes;
- Leve e rápido:

**Sempre visitar a documentação de determinado código**

**ALGUNS** **COMANDOS:**

Git clone⇒ Clona um repositório Git existente para um novo diretório(pasta)local

Git commit⇒ Grava alterações no repositório.

Git pull⇒ Puxa as alterações do repositório remoto para o local(busca e mescla)

Git push⇒ empurra as alterações do repositório local para o remoto

**O que é GitHub?**

- Comunidade ativa;
- Utilizado mundialmente;
- Mascote “Octocat”:

**AULA 2⇒ Instalação, Configuração e Autenticação**

**Instalação⇒**

Windows⇒ No site do GIT

Linux⇒ Por linhas de comando

**Configuração⇒**

Comandos importantes> Git config, Git config init.defaultBranch

**⇒ Documentation**

- Armazenar o email e senha no global;

**Autenticando via Token⇒**

—Aula prática—

—Credential.helper store(salva a autenticação);

 —  —show-origin (mostra o que tem dentro da variável) ;

— cat exibe o conteúdo dentro do arquivo depois de já dentro do arquivo;

**Autenticando via chave SSH⇒**

—Tem como ver os passos pelo GitHub;

— Para conferir se há chaves SSH na máquina, é necessário usar o comando: ls -a -/.ssh;

**AULA 3- Primeiros passos com Git e GitHub⇒**

**Criando e Clonando Repositórios⇒**

- Transformando um diretório local que não está sob controle de versão, num repositório Git;
- Clonando um repositório Git existente:

- mkdir= cria uma pasta;
- Git remote add origin Url= Conecta a pasta local com o repositório remoto;
- Git clone Url nome-do-diretório local= cria um clone do repositório;
- Git clone Url —branch nome-da-branch —single-branch;

**Criando um repositório no GitHub⇒**

- README= Dá uma descrição maior a respeito do projeto;
- .gitignore= ignorar arquivos;
- License= Liberdade usual do seu código

**Salvando Alterações no Repositório Local⇒**

- Para criarmos uma pasta é necessário usar o comando mkdir, logo após isso, adicionamos os arquivos restantes com o comando touch;
- Para colocarmos os arquivos na área de preparação, é preciso usar o comando git add;
- Para tirarmos o arquivo da preparação e dar um commit é preciso usar o comando git commit -m “mensagem”;
- Para conferirmos mais a respeito dos status do repositório git, é essencial usarmos o git status;
- Podemos usar o .gitignore para podermos ignorar algum arquivo ou pasta, usando o comando echo nome-da-pasta/> .gitignore;
- Usando o git log, vemos o histórico de commit’s:

**Desfazendo alterações no repositório local⇒**

- Para remover a extensão git na pasta basta usar o comando rm -rf nome-da-extensão;
- Para descartarmos uma alteração em determinado repositório, precisamos usar o comando git restore;
- Para mudarmos um commit feito de forma errada, basta usarmos o git commit —amend -m”adicionando” uma nova mensagem”;
- Para deletarmos um commit usamos o comando git reset -(mixed, hard, soft);
- Com o comando relog podemos visualizar mais detalhadamente o histórico de commit’s;

**Enviando e Baixando alterações no repositório remoto⇒**

- Para enviar alterações para o nosso repositório remoto, é preciso clonar o repositório(git clone e cd);
- Após isso, entramos nele e adicionamos o arquivo que queremos(git add e git commit);
- Logo depois, para empurrar as informações para o repositório, usamos o comando git push origin branch(main):

**Trabalhando com Branches Criando, Mesclando, Deletando e Tratando Conflitos⇒**

**Trabalhando com Branches⇒**

- Uma branch é a ramificação do seu projeto;
- É um ponteiro móvel para um commit no histórico do repositório;
- Quando você cria uma nova branch a partir de outra existente, a nova se inicia apontando para o mesmo commit da branch que estava quando foi criada;

**Mesclando⇒**

- Para criar uma branch é necessário usar o comando git checkout -b nome-da-branch;
- Depois disso, as alterações feitas serão adicionadas na branch criada;
- Para voltar para a branch antiga, é preciso usar  o comando git checkout nome-da-branch-antiga;
- Para ver as branch e seus últimos commit’s, é preciso usar os comandos git branch e git branch -v;
- Para deletar uma branch, usamos o comando git branch -d nome-da-branch:

**Comandos uteis no dia a dia⇒**

- Se você quiser apenas baixar o conteúdo da commit, é possível usar o comando git fetch origin main, depois disso, é usado o comando git diff main/origin main, e depois é mesclado com git merge origin/main;
- Para clonar apenas uma branch do repositório, basta usarmos o comando git clone Url —branch nome-da-branch —single-branch;
- Também podemos usar o comando git stash para arquivar uma modificação feita, e usando o git stash list, podemos observar um pouco a respeito da lista de modificações arquivadas e para voltarmos com as modificações, usamos o git stash(apply ou pop);

**PARA EVOLUIR MAIS NO USO DO GIT É RECOMENDADO A DOCUMENTAÇÃO DO SITE!**

GitFluence⇒ IA útil

GitHub útil:

https://github.com/elidianaandrade/dio-curso-git-github

Slides úteis:

https://academiapme-my.sharepoint.com/:p:/g/personal/renato_dio_me/EYjkgVZuUv5HsVgJUEPv1_oB_QWs8MFBY_PBQ2UAtLqucg?rtime=VabaNmrS20g
