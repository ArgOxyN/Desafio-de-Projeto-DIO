# Teoria por trás dos comandos básicos do Git

Git INIT: Cria um diretório dentro da sua biblioteca do Git

Git ADD: Move um arquivo para dentro da sua biblioteca diretamente ao ponto “Staged”.

Um arquivo UNTRACKED ainda não está presente na sua biblioteca.

Um arquivo TRACKED já está presente em sua biblioteca, mas pode ser interpretado de diversas maneiras:

- Unmodified: Um arquivo inalterado desde sua adição à biblioteca.
- Modified: Um arquivo alterado previamente.
- Staged: Um arquivo que está sendo preparado.
- Commit: A camada mais profunda que engloba os chamados “objetos” dentro de um diretório Git (Sendo eles: Commit, Tree, Blob).
- Tree: Trees podem armazenar outras trees, ou blobs.
- Blob: armazenam arquivos dentro do seu diretório Git.

Git COMMIT: Encripta toda uma cadeia de objetos em uma Commit através de uma SHA1 (Security Hash Algorithm v1), retornando todos esses arquivos ao estado Unmodified.

Git STATUS: Imprime os status atuais de cada arquivo dentro da sua “Working Tree” e te notifica se há algo à ser “Commitado”.

Git RESTORE: Restaura um arquivo à um estado anterior listado no “git status”.

**Pontos Importantes**

- O seu ambiente de trabalho consiste em duas áreas distintas sendo o Desk (seu computador), e o Git que não faz atualização desses dados anteriormente salvos imediatamente exceto que haja à interferência de um código em específico.
- Cada camada entre os objetos possui uma diferente encriptação em SHA1, cada Blob, Tree ou Commit específico possui um diferente ID de 40 dígitos distintos que se alteram com a mudança de qualquer caractere dentro do arquivo.
