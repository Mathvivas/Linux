## Compactadores

- São programas que diminuem o tamanho de um arquivo ou diretório.

## Extensões

- Identificam o tipo de um arquivo e o programa necessário para manipular o mesmo.

# Compactadores

## gzip

- Muito usado, possui uma taxa excelente de compactação.

- gzip arquivo.txt
- gzip -9 arquivo.txt: Usa a compactação máxima; Usar para arquivos enormes

## zip

- zip arquivo.zip arquivo.txt
- zip arquivos.zip arquivo1.txt arquivo2.txt ...
- Para zippar todos os arquivos de um diretório:
  - zip -r arquivo.zip *

## bzip2

- bzip2 arquivo.txt

## rar

- rar a arquivo.rar arquivo.txt



# Descompactação

## gunzip

- gunzip arquivo.txt.gz
- Para redirecionar a compressão para um arquivo:
    - gzip -c arquivo.txt > arquivo.txt.bz

## unzip

- unzip arquivo.zip

## bzip2

- bzip2 -d arquivo.bz2

## rar

- rar x arquivo.rar

## tar.gz

- tar -xvf arquivos.txt.tar.gz



# Arquivadores

- Junta vários arquivos em um só, mas pode ser usado em conjunto com um compactador para
armazenar arquivos compactados.

## tar

- tar -cf arquivos.txt.tar arquivo1.txt arquivo2.txt ...
- tar -tf arquivo.tar : Lista o conteúdo arquivado.

- Para comprimir com gzip:
```bash
tar -czvf arquivo.tar.gz arquivo1.txt arquivo2.txt ...
```

- Para comprimir com bzip2:
```bash
tar -cjvf arquivo.tar.bz arquivo1.txt arquivo2.txt ...
```