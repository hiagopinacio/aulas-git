git Add e git Commit
====================

Mudar Diretorios
----------------

Ir para diretório:

	cd diretorio/diretorio2

Voltar Diretório:

	cd ..

Listar arquivos do diretório atual:

	ls


Criar Repositório
-----------------

1 - abrir git bash

2 - ir para a pasta do projeto

	cd <dir>

3 - Digitar o comando:
	
	git init


Verificando o Status do Repositório:
------------------------------------

	git status

Verifica se tem alterações realizadas nos arquivos dentro do reposítório.

Adicionar Arquivos Alterados Para *Staging Area*
----------------------------------------------------

#### Adicionar um arquivo especifico:

	git add arquivo.txt

#### Adicionar arquivos com algum nome em comum:

	git add *.txt 

adiciona todos os arquivos que terminam com .txt.

#### Adicionar todos os arquivos do repositório:

		git add .

### Após add arquivos

	git status

mostra arquivos na *staging area* prontos para serem commitados.



Registrar Estado do Código (commit):
------------------------------------

	git commit -m "mensagem para identificação"

Após commitar 'git status' mostra que o repositório está atualizadose não há mais nada para commitar

Para adicionar todos os arquivos e realizar commit em uma linha:
	
	git commit -a -m "mensagem de identificação"

Ignorando Arquivos Dentro do Projeto
------------------------------------

1. Criar um arquivo chamado .gitignore
2. Inserir neste arquivo todos os arquivos a serem ignorados (1 por linha)

Desta forma o comando ***git add .*** ignorará os arquivos listados.
