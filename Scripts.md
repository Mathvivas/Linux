# Scripts

- Para executar um script utilizando o interpretador <strong>bash</strong> :

```bash
bash script.sh
```

- Ao adicionar a permissão de execução :

```bash
caminho/script.sh
```

## Shebang (#!)

- Indicam com qual programa iremos executar o script;
- Colocado no início do script.

```sh
#!/bin/bash
```

- Em um script Ruby:

```txt
#!/usr/bin/ruby

puts "Olá, Ruby!"
```

## source

- Quando não executamos source, inicia-se um processo filho, ou seja, as variáveis criadas nesse processo são criadas e eliminadas no mesmo, sem conexão com o processo pai;

- Ao executar com o source, não inicia-se o processo filho, ou seja, as variáveis criadas permanecem;

```bash
source script.sh
```
______________________

## Argumentos e Aspas

- Podem ser colocados argumentos após o script:

```bash
script.sh 2020 logs Matheus
```

- Esses argumentos podem ser usados ou não;
- No script:

```sh
#!/bin/bash

echo ${0}   # Representa o próprio script (caminho para o script)
echo $#     # Número de Argumentos
echo $*     # Mostra todos os argumentos
echo ${1}   # Primeiro Argumento
echo ${2}   # Segundo Argumento
echo ${3}   # Terceiro Argumento

echo "Compactando os logs de ${1} em `pwd`."
echo "Meu nome é ${3}."
echo 'Meu nome é ${3}.'

echo "pwd"      # Retorna pwd
echo "`pwd`"    # Retorna o caminho
```

- Aspas Duplas interpretam variáveis;
- Aspas Simples não interpretam variáveis.


## For Loops

```sh
#!/bin/bash

# arquivo.sh ANO [ANO...]
# No mínimo 1 ano, mas suporta diversos anos

for ANO in 2016 2017
do
    echo "Compactando os logs de ${ANO} em `pwd`."
done

```

```sh
#!/bin/bash

# arquivo.sh ANO [ANO...]
# No mínimo 1 ano, mas suporta diversos anos

for ANO in $*       # Para todos os argumentos passados
do
    echo "Compactando os logs de ${ANO} em `pwd`."
done

```

```sh
#!/bin/bash

lista='banana maca chocolate'
for i in $lista
do
    echo $i
done
```

## Editores de Texto

### vi

- vi <i>arquivo.extensão</i> : Cria o arquivo
- Após entrar no editor vi: 
  - digitar :set number para numerar as linhas
  - :wq para Salvar e sair do vi

### nano

- nano <i>arquivo</i>: Edita o arquivo no próprio Shell.
- ^ = Ctrl
- M = Alt
- Ctrl ^ = Seleciona uma palavra