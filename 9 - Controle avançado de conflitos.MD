Controle de Conflitos
=====================

Tranzendo um commit específico de outra branch:
-----------------------------------------------

Na branch onde será aplicada a alteração:

    git cherry-pick {Chave-do-commit}

Assim, quando finalizar as alterações da outra brach, o git entende que uma alteração já foi sincronizada, e não terá conflito.
Isto é melhor do que fazer a mesma alteração  duas vezes em dois branches diferentes.

Encontrando o estado do código desejado
---------------------------------------

Para iniciar uma busca em uma série de commits:

    git bisect start

Inicialmente, é preciso informar um estado, ou commit cuja parte do código que queremos não esteja boa:

    git bisect bad HEAD

em seguida devemos informar o estado em que possivelmente estava bom:

    git bisect good {chave do ultimo commit de busca}

Com isso, será carragado um estado do código, se este estado for o desejável, deve ser executado:

    git bisect good

> se digitar git bisect bad, ele continuará buscando e carregando outros estados do código dentro do intervalo de busca.

Com o fim da busca, o git mostrará a chave do commit encontrado.

Para voltar ao master: 

    git bisect reset

É sempre bom verificar todas as alterações deste commit antes de reverter para ele:

    git show {chave do commit desejado}
    
E para aplicar as alterações do commit encontrado:

    git reset {chave do commit desejado}


Encontrar responsáveis por alteração
------------------------------------

através do comando:

    git blame arquivo.txt

será exibido quem e quando foir realizada a alteração de cada linha do arquivo.txt