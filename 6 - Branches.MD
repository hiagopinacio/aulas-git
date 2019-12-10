Branches
========

CRIANDO BRANCHES
----------------

Para criar um branch chamado teste:

    git branch teste

Para mudar o branch de tabalho de master para teste:

    git checkout teste 

Para criar um branch e ir para ele, pode utilizar o seguinte comando:

    git checkout -b teste

MERGE
-----

Para unir dois branches:

1 - voltar para o branch padrão:
    
    git checkout master

2 - trazer as alterações em teste para o branch atual
    
    git merge teste

3 - apagar o branch

    git branch -d teste

### Caso haja conflito no merge

ex.: um arquivo foi alterado em teste e depois foi alterado no branch master antes do merge

 > As diferenças ficam salvas no arquivo conflintante, sendo necessário concertar manualmente antes de commitar depois.S

