Repositório em Rede
===================

Criando Repositório
-------------------

Na maquina principal:

	git init --bare
	
>o ***--bare*** indica que não é um repositório de trabalho, guardando apenas as alterações no repositório. Com isso outros usuarios do servidor podem fazer alterações nele.

Acessando o repositório
-----------------------
primeiro acesso no repositorio de um outro usuário: precisa dar clone

	git clone file:////servidor/path_no_servidor <nome_dir> 
	
> clona o projeto do servidor para *nome_dir* no path atual

Nome do repositório remoto dentro do seu git

	git remote
	> origin

Por padrão ***origin*** é o nome criado pelo git para repositórios remotos.

Para aplicar alterações, é necessário commitar as mudanças:

	git commit -m "mensagem"

> essa alteração é salva apenas no repositório local.

Para enviar as mudanças para o servidor:

	git push origin master
	
> manda os dados para o servidor utilizando o remoto origin do branch master

