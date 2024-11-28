
# CURSO IFPR DE GIT E GITHUB

Git é uma ferramenta de repositório e controle de versão lançada em 2005, criada por Linus Torvalds. Hoje em dia o git contém serviços de repositórios remotos acessados pela ferramente como o GitHub da Microsoft e o GitLab de código aberto.

O git funciona por uma estrutura de árvore, ou linha, exisitindo um repositório principal chamado de MAIN (Antigamente MASTER), essa "branch" pode ser duplicada, clonada e alterada por múltiplas pessoas ao mesmo tempo, além de oferecer um retorno para uma versão antiga caso um repostório local (ou seja clonado em uma máquina) esteja disponível.

O fluxo principal do git é baseado em alterar, examinar o histórico e adicionar mudanças a branchs secundárias e a main, colaborando com outros que realizam os mesmos passos.

O git utiliza principalmente o prompt de comando Bash para a navegação entre diretórios, mas utiliza de comandos próprios para a manipulação própria da ferramenta, exemplo de um ciclo comum de git seria:

- git init (Incializa o git no diretório)

- git add . (adiciona os arquivos e pastas do diretório a branch local, o ponto sinalizando para adicionar todos os arquivos a branch temporária)

- git commit -m (realiza um "commit", se compromentendo a alterar aquilo que foi adicionado ou removido)

- git push -u origin main (altera os arquivos no repositório origem, na branch main)

# GIT BRANCH

Uma branch é uma ramificação de um projeto, ao invés de alterar linha "main" uma branch é criada para criar um ambiente que possa ser alterado sem a possibilidade de quebrar alguma funcionalidade séria.

```
	 _____@commit_____@commit_______@commit____________ Branch "Teste"
	/

@commit-------------@commit---------------------@commit---------------------- Main

        \_________@commit______@commit___________/ Branch "Teste" (Merged)

```

- git branch name (cria uma branch)

- git checkout name (troca de branch)

- git branch (lista as branchs)

- git branch -v (mostra as mudancas das branchs)

- git branch -d nome (deleta a branch, se a flag -d for escrita em maiúsculo "-D" a remoção será deletada sem perguntar)

- git reset -flag (Reseta o código para um ponto anterior)

## Nomenclatura

nomes de branch em snake-case

- feature - se é alguma nova funcionalidade

- fix - se está para consertar um erro da main

- test - se é para teste

- git push -u origin main (altera os arquivos no repositório origem, na branch main)

# GIT RESETTING

Para realizar controle de versões e especialmente o rollback de versões, se utiliza o comando git reset.

Para se utilizar o git reset utiliza o padrão de comando 

``` git reset --flag commitcode ```

O código de commit é ilustrado como uma string que aparece junto ao commit ao digitar git log.
A existem três flags para o reset, essas são:

- --soft (Irá retornar a "cabeça" (HEAD), para o commit, mas não deleta nenhum outro commit)
- --mixed (Irá resetar a HEAD, e não deleta arquivos, mas não marca nenhum arquivo removido para ser adicionado junto ao commit)
- --hard (Simplesmente deleta os arquivos e posiciona a HEAD para o commit)

