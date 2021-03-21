# Comandos do Terminal

## pwd

- pwd: Caminho percorrido até a pasta atual.

## ls

- ls: Lista o que tem dentro da pasta atual.
- ls <i>diretório</i>: Lista o que tem dentro do diretório.
- ls -l: Lista os detalhes dos diretórios.
- ls -F : Mostra os arquivos e diretórios de uma forma visual, não por cores.
- ls --sort=size : Lista pelo tamanho dos arquivos.
- ls * : lista o conteúdo de todos os diretórios dentro do diretório atual.

## cd

- cd <i>diretório</i>: Muda para o diretório.
- cd .. : Retorna para o diretório anterior.
- cd ~: Retorna para o diretório pessoal.
- cd /: Entra no diretório raiz.
- Ao digitar cd sem argumentos, retornamos ao diretório home do usuário.

## mkdir

- mkdir <i>diretório</i>: Cria um diretório.
- mkdir -p diretório1/diretório2/diretório3 : Cria todos os diretórios, se não existirem.

## man

- man <i>comando</i>: Gera o manual do comando;
- Na tela do Manual:
  - /Comando: Busca o comando desejado;
  - 'n' para passar pelas buscas.

## less

- Visualizador de arquivos, semelhante ao man;
- less arquivo.txt.

## find

- Procura tudo o que está em certo diretório:
  - find /Documents
- Para procurar pelo nome:
  - find -name "log*" : Tudo que começa com log
  - find -name "*g\*" : Tudo que tem g no meio
- Para achar somente diretórios:
  - find -type d -name "*user\*"
- Para achar somente arquivos:
  - find -type f -name "*user\*"
- Para achar pelo tamanho de pelo menos 1000k:
  - find -size +1000k
- Para achar os arquivos que foram acessados nos últimos 7 dias:
  - find -atime -7
- Para achar os arquivos que foram modificados nos últimos 7 dias:
  - find -mtime -7
- Para achar arquivos com OR (por padrão, é AND):
  - find -name "*log\*" -o -name "2016\*"
- Para achar arquivos que tenham log e não tenham 2016:
  - find -namee "*log\*" ! -name "*2016\*"
- Para ignorar maiúsculo e minúsculo:
  - find -iname
- Para executar outro comando para CADA resultado:
  - find -name "*log\*" -name "*2016\*" -exec echo '{}' foi encontrado ";"

## locate

- locate arquivo;
- Procura pelo sistema de arquivos inteiro;
- <strong>Possui um banco de dados próprio com todos os arquivos.</strong> Gera uma busca rápida.
- Após criar ou remover um arquivo, é necessário atualizar o banco de dados:
  - sudo updatedb.

## mv

- mv antigo nome novo nome: Modifica o nome
- mv arquivo [caminho do diretório]: Move o arquivo

## touch

- touch <i>arquivo.extensão</i>: Cria um arquivo vazio.

## cp

- cp arquivo.extensão caminho do diretório: Copia o arquivo no diretório indicado.

## rm

- rm <i>arquivo</i>: Remove o arquivo.
- rm -r <i>diretório</i>: Remove o diretório.

## whereis

- Retorna o caminho até o arquivo.

## nano

- nano <i>arquivo</i>: Edita o arquivo no próprio Shell.
^ = Ctrl
M = Alt

## cat

- cat <i>arquivo</i>: Lê o arquivo.
- tac <i>arquivo</i>: Lê o arquivo de baixo para cima.
- head <i>arquivo</i>: Lê as 10 primeiras linhas do arquivo.
- tail <i>arquivo</i>: Lê as 10 últimas linhas do arquivo.

## chmod

- chmod +x <i>arquivo.extensão</i> : Torna o arquivo executável

## vi

- vi <i>arquivo.extensão</i> : Cria o arquivo
- Após entrar no editor vi: 
  - digitar :set number para numerar as linhas
  - :wq para Salvar e sair do vi

## > e >>

- '>' : Substitui.
- '>>' : Adiciona.
- tail arquivo.txt > teste.txt: Copia as úlimas 10 linhas do arquivo.txt no teste.txt.
- cal maio 2020 > maio.txt

## cal

- cal: Mostra o calendário do mês.
- cal <i>ano</i>: Mostra o calendário do ano todo.
- cal <i>mês ano</i>: Mostra o calendário do mês do ano.

## date

- Mostra o data

## | (pipe) e grep

- tail arquivo.txt | grep <i>palavra</i>: Procura a 'palavra' no arquivo.txt.

## & e &&

- cat arquivo.txt & cat arquivo2.txt: Mostra os arquivos separadamente.
- cat arquivo.txt && cat arquivo2.txt: Mostra os arquivos em uma saída.
- mkdir linux && cd linux: Cria e entra direto.

## file

- file <i>arquivo</i>: Mostra qu tipo de arquivo é.

## find

- find ~ -name teste.txt: Procura o arquivo teste.txt pelo nome no diretório pessoal e retorna o caminho.

## lsusb

- Lista os componentes conectados via usb.

## uname

- Nome do Kernel.

## uname -r

- Versão do Kernel.

## lscpu

- Visualiza os dados da CPU.

## lshw -short

- Exibe informações sobre o hardware.

## echo

- echo -e "---Informações de Hardware---\n": Printa essa string (com a quebra de linha) no terminal.

## type

- type comando;
- type -t comando
  - Mostra somente a palavra que descreve.

## !!

- Executa o último comando utilizado.

## Ctrl + W

- Apaga uma palavra na linha atual.

## Ctrl + U

- Apaga a linha inteira.

## exit ou Ctrl + D

- Sai do terminal

## Ctrl + Z

- Interrompe a execução do comando.

## clear ou Ctrl + l

- Limpa o terminal

## echo $?

- Diz qual foi o resultado do último comando;
- 0: Tudo certo;
- 1: Erros no geral;
- 127: Comando não encontrado;
- 130: Script terminado por Ctrl-C

## *

- Tendo vários arquivos de texto:
  - cat *.txt
  - ls *.txt

## ?

- ? pega <strong>somente</strong> um caractér ou número;
- Tendo vários arquivos textoN.txt, onde N é um número:
  - cat texto?.txt
  - Se N >= 10, não é selecionado, pois possui 2 números e o "?" pega somente 1.
  - cat texto[0-5].txt: Retorna os texto0.txt ao texto5.txt;
  - cat {texto[a-z].txt, texto[A-Z].txt}: Pega os dois padrões.

## ;

- Possibilidade de executar vários comandos

```bash
ls ; echo 'Listagem Completa'

echo 'Minha mensagem' ; echo 'Minha outra mensagem'
```

___________________

<br>

## Shell

- <strong>Bash</strong> é o interpretador <strong>shell</strong> mais famoso;
  
- Outros exemplos são: csh e sh