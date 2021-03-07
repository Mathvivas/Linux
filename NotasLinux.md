* O Linux é o Kernel ou Núcleo do Sistema Operacional;

* Criado em 1991 por Linus Torvalds;

* Existem diversas distrubuições para diversos fins;

* O terminal, ou Shell é uma linha de comando onde podemos executar programas específicos do Linux.

## Comandos do Shell

### pwd

* pwd: Caminho percorrido até a pasta atual.

### ls

* ls: Lista o que tem dentro da pasta atual.
* ls [diretório]: Lista o que tem dentro do diretório.
* ls -l: Lista os detalhes dos diretórios.

### cd

* cd [diretório]: Muda para o diretório.
* cd .. : Retorna para o diretório anterior.
* cd ~: Retorna para o diretório pessoal.
* cd /: Entra no diretório raiz.

### mkdir

* mkdir [diretório]: Cria um diretório.

### man

* man [comando]: Gera o manual do comando.

### mv

* mv antigo nome novo nome: Modifica o nome
* mv arquivo [caminho do diretório]: Move o arquivo

### touch

* touch [arquivo.extensão]: Cria um arquivo vazio.

### cp

* cp arquivo.extensão caminho do diretório: Copia o arquivo no diretório indicado.

### rm

* rm [arquivo]: Remove o arquivo.
* rm -r [diretório]: Remove o diretório.

### nano

* nano [arquivo]: Edita o arquivo no próprio Shell.
^ = Ctrl
M = Alt

### cat

* cat [arquivo]: Lê o arquivo.
* tac [arquivo]: Lê o arquivo de baixo para cima.
* head [arquivo]: Lê as 10 primeiras linhas do arquivo.
* tail [arquivo]: Lê as 10 últimas linhas do arquivo.

### > e >>

* > : Substitui.
* >> : Adiciona.
* tail arquivo.txt > teste.txt: Copia as úlimas 10 linhas do arquivo.txt no teste.txt.
* cal maio 2020 > maio.txt

### cal

* cal: Mostra o calendário do mês.
* cal [ano]: Mostra o calendário do ano todo.
* cal [mês ano]: Mostra o calendário do mês do ano.

### date

Mostra o data

### | (pipe) e grep

* tail arquivo.txt | grep [palavra]: Procura a 'palavra' no arquivo.txt.

### & e &&

* cat arquivo.txt & cat arquivo2.txt: Mostra os arquivos separadamente.
* cat arquivo.txt && cat arquivo2.txt: Mostra os arquivos em uma saída.
* mkdir linux && cd linux: Cria e entra direto.

### file

* file [arquivo]: Mostra qu tipo de arquivo é.

### find

* find ~ -name teste.txt: Procura o arquivo teste.txt pelo nome no diretório pessoal e retorna o caminho.

### lsusb

Lista os componentes conectados via usb.

### uname

Nome do Kernel.

### uname -r

Versão do Kernel.

### lscpu

Visualiza os dados da CPU.

### lshw -short

Exibe informações sobre o hardware.

### echo

* echo -e "---Informações de Hardware---\n": Printa essa string (com a quebra de linha) no terminal.

=============================================================================================================

## Atalhos do Shell

### !!

Executa o último comando utilizado.

### Ctrl + W

Apaga uma palavra na linha atual.

### Ctrl + U

Apaga a linha inteira.

### exit ou Ctrl + D

Sai do terminal

### Ctrl + Z

Interrompe a execução do comando.

### clear ou Ctrl + l

Limpa o terminal

=============================================================================================================

## Diretórios

### /bin/

Binários principais do sistema;
Comando cd;

### /boot/

Arquivos do sistema Boot;
Arquivos para carregar e inicializar o S.O.;

### /dev/

Arquivos de dispositivos;

### /etc/

Arquivos de configuração do sistema;

### /home/

Diretório dos usuários comuns do sistema;

### /lib/

Bibliotecas essenciais do sistema e os módulos do Kernel;

### /media/

Diretório de montagem de dispositivos;

### /mnt/

Diretório de montagem de dispositivos;

### /opt/

Instalação de programas não oficiais da distribuição ou por conta do usuário;

### /sbin/

Armazena arquivos executáveis que representam comandos administrativos. Ex: shutdown;

### /srv/

Diretório para dados de serviços fornecidos pelo sistema;

### /tmp/

Diretório para arquivos temporários;

### /urs/

Segunda hierarquia do sistema, onde ficam os usuários comuns do sistema e programas;

### /var/

Diretório com arquivos variáveis gerados pelos programas do sistema;

### /root/

Usuário root. Possui total poder sobre o sistema;

### /proc/

Diretório virtual controlado pelo Kernel;
cpu info.


