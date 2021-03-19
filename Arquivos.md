## Compactadores

- São programas que diminuem o tamanho de um arquivo ou diretório.

## Extensões

- Identificam o tipo de um arquivo e o programa necessário para manipular o mesmo.

## Compactadores

### gzip

- Muito usado, possui uma taxa excelente de compactação.

- gzip arquivo.txt
- gzip -9 arquivo.txt: Usa a compactação máxima; Usar para arquivos enormes

### zip

- zip arquivo.zip arquivo.txt
- zip arquivos.zip arquivo1.txt arquivo2.txt ...

### bzip2

- bzip2 arquivo.txt

### rar

- rar a arquivo.rar arquivo.txt



## Descompactação

### gunzip

- gunzip arquivo.txt.gz

### unzip

- unzip arquivo.zip

### bzip2

- bzip2 -d arquivo.bz2

### rar

- rar x arquivo.rar

### tar.gz

- tar -xvf arquivos.txt.tar.gz



## Arquivadores

- Junta vários arquivos em um só, mas pode ser usado em conjunto com um compactador para
armazenar arquivos compactados.

### tar

- tar -cf arquivos.txt.tar arquivo1.txt arquivo2.txt ...

