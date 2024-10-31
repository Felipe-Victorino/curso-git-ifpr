# Branch

Uma branch é uma ramificação de um projeto, ao invés de alterar linha "main" uma branch é criada para criar um ambiente que possa ser alterado sem a possibilidade de quebrar alguma funcionalidade séria.

´´´
	 _____@commit_____@commit_______@commit____________ Branch "Teste"
	/

@commit-------------@commit---------------------@commit---------------------- Main

        \_________@commit______@commit___________/ Branch "Teste" (Merged)

´´´

- git branch name (cria uma branch)

- git checkout name (troca de branch)

- git branch (lista as branchs)

- git branch -v (mostra as mudancasdas branchs)

- git branch -d nome (deleta a branch, se a flag -d for escrita em maiúsculo "-D" a remoção será deletada sem perguntar)