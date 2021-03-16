# Comandos do Terminal

## pwd

- pwd: Caminho percorrido até a pasta atual.

## ls

- ls: Lista o que tem dentro da pasta atual.
- ls <i>diretório</i>: Lista o que tem dentro do diretório.
- ls -l: Lista os detalhes dos diretórios.

## cd

- cd <i>diretório</i>: Muda para o diretório.
- cd .. : Retorna para o diretório anterior.
- cd ~: Retorna para o diretório pessoal.
- cd /: Entra no diretório raiz.

## mkdir

- mkdir <i>diretório</i>: Cria um diretório.

## man

- man <i>comando</i>: Gera o manual do comando.

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

