Editando Alterações
===================

Editando o Ultimo Commit
------------------------

    git add .
    git commit --amend -m "mensagem(edição)" 

Isto commita alteração junto com o útimo sem criar um novo

Unir Commits
------------
Para unir os ultimos 3 commits pro exemplo, pode-se usar o seguinte comando:

    git rebase -i HEAD~3

ou 

    git rebase -i {chave}

Com isso, irá aparecer uma lista dos commits selecionados, do mais antigo para o mais novo.

Ao trocar o parâmetro ***pick*** por ***s***, os commits marcado com ***s*** serão unidos no último commit marcado com ***pick***.

Para salvar, basta digitar:
    
    :x

Então, será necessário editar a mensagem do commit, e novamente, para salvar e sair, utilizar:

    :x



Remover Arquivo da Staging Area
-------------------------------

Caso tenha executado um ***git add*** errado, é possível remove-lo da *stagin area* com o seguinte comando:
    
    git reset HEAD arquivo.txt
    
Neste exemplo, o arquivo.txt seria removido.

Desfazendo Mudanças nos arquivos
--------------------------------

voltando ao estado do ultimo commit

    git checkout -- arquivo.java 

Isto modifica o arquivo e descarta todas as alterações feitas após o último commit

Remover arquivos do repositório
-------------------------------

Para remover arquivos do repositório após um git add em que arquivos foram removidos:

    git rm arquivo.txt

