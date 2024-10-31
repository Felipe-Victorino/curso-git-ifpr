# CURSO IFPR DE GIT E GITHUB

Git é uma ferramenta de repositório e controle de versão lançada em 2005, criada por Linus Torvalds. Hoje em dia o git contém serviços de repositórios remotos acessados pela ferramente como o GitHub da Microsoft e o GitLab de código aberto.

O git funciona por uma estrutura de árvore, ou linha, exisitindo um repositório principal chamado de MAIN (Antigamente MASTER), essa "branch" pode ser duplicada, clonada e alterada por múltiplas pessoas ao mesmo tempo, além de oferecer um retorno para uma versão antiga caso um repostório local (ou seja clonado em uma máquina) esteja disponível.

O fluxo principal do git é baseado em alterar, examinar o histórico e adicionar mudanças a branchs secundárias e a main, colaborando com outros que realizam os mesmos passos.

O git utiliza principalmente o prompt de comando Bash para a navegação entre diretórios, mas utiliza de comandos próprios para a manipulação própria da ferramenta, exemplo de um ciclo comum de git seria:

- git init (Incializa o git no diretório)

- git add . (adiciona os arquivos e pastas do diretório a branch local, o ponto sinalizando para adicionar todos os arquivos a branch temporária)

- git commit -m (realiza um "commit", se compromentendo a alterar aquilo que foi adicionado ou removido)

- git push -u origin main (altera os arquivos no repositório origem, na branch main)