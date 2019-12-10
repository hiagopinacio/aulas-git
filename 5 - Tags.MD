TAGs
====

Criar TAG
---------

    git tag -a <TAG> -m "mensagem"
    
O parâmetro ***-a*** serve para criar tag anotada com usuario e horario...

Criar tag para commits antigos
------------------------------

    git tag -a v0.0 <CHAVE DO COMMIT> -m "mensagem. ex.: versao 0.0"

Consutar Tags:
--------------

    git tag

Consultando Detalhes Sobre Uma Tag:
-----------------------------------

    git show <TAG>


Restaurando uma Versao Anterior dos Arquivos pela Tag
-----------------------------------------------------
 
    git checkout <TAG>

Deletando a Tag:
----------------

    git tag -d <TAG>
