Consultando Alterações na Pasta do Projeto
==========================================

Mostrar alterações realizadas nos arquivos e que ainda nao foram adicionados

	git diff # 

>-vermelho mostra o que foi removido

>+verde mostra o que foi adicionado

É possível ver as alterações realizadas nos arquivos adicionados na staging área através do seguinte comando:

	git diff --staged

para verificar alterações em um commit anterior:

	git show {chave-do-commit}

Histórico de Commits
--------------------

Para listar todos os commits realizados:

	git log

Utilizando o parâmetro **-p** mostra as alterações realizadas em cada commit

	git log -p

Para sair do log criado, basta digitar **q**

Para vizualizar os últimos **n** commits, basta passar -n como parâmetro do comando.
ex.:

	git log -p -2


"Interface para vizualizar as alterações no repositório"
--------------------------------------------------------

O vizualizador de relatórios de modificações pode ser acessado dentro do repositório através do seguinte comando:

	gitk