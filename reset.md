# GIT Resetting

Para realizar controle de versões e especialmente o rollback de versões, se utiliza o comando git reset.

Para se utilizar o git reset utiliza o padrão de comando 

``` git reset --flag commitcode ```

O código de commit é ilustrado como uma string que aparece junto ao commit ao digitar git log.
A existem três flags para o reset, essas são:

- --soft (Irá retornar a "cabeça" (HEAD), para o commit, mas não deleta nenhum outro commit)
- --mixed (Irá resetar a HEAD, e não deleta arquivos, mas não marca nenhum arquivo removido para ser adicionado junto ao commit)
- --hard (Simplesmente deleta os arquivos e posiciona a HEAD para o commit)
