## wc

* wc -l [arquivo]: Número de linhas do arquivo
* wc -w [arquivo]: Número de palavras do arquivo
* wc -c [arquivo]: Número de bytes do arquivo
* wc -m [arquivo]: Número de chars do arquivo

## cowsay

* cowsay "Linux é bom"
* cowsay -d ""
* cowsay -g ""
* cowsay -f tux "": Pinguim
* cowsay -f vader ""
* cowsay -f vader-koala ""
* cowsay -f dragon ""

## xcowsay

* xcowsay ""

## cmatrix

Efeito do filme

## init 0

Desliga o computador

## seq

Sequência de números
* seq 1 10

## Usuário

su [nome do usuário]: Troca para este usuário
adduser [nome do usuário]: Adiciona um usuário

Se não possuir permissão, adicionar 'sudo' antes dos comandos: sudo su, sudo adduser

## ls -lh

Verifica as permissões do diretório
r: read; w: write; x: execution

* Primeiro Símbolo: d (diretório), - (arquivo)
* Segundo ao Quarto Símbolo: Permissões do dono
* Quinto ao Sétimo Símbolo: Permissões do grupo
* Oitavo ao Décimo Símbolo: Permissões para outros

## chmod

* Modo Octal: 0 (nenhuma permissão) a 7 (permissão total)
* Mudar a permissão de um arquivo ou diretório
* O primeiro dígito representa o dono (u)
* O segundo dígito representa o grupo (g)
* O terceiro dígito representa os outros (o)

read = 4
write = 2
execute = 1

* chmod 200 [arquivo]: Somente o dono pode escrever no arquivo
* chmod 300 [arquivo]: Somente o dono pode escrever e executar (2 + 1) no arquivo
* chmod 700 [arquivo]: Somente o dono possui todas as permissões
* chmod 754 [arquivo]: Dono possui todas as permissõs; Grupo pode ler e executar; Outros podem ler


