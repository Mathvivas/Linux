- Pacotes são programas colocados dentro de um arquivo identificado por sua extensão, e
incluem arquivos necessários para a instalação do programa.

- Extensões: .deb, .rpm

# Gerenciadores

- São sistemas que possuem resolução automática de dependências entre pacotes, método
fácil de instalação de pacotes.

- Exemplos: dpgk, apt, yum

# Instalação e Remoção

## apt

- Gerencia, busca pacotes

- sudo apt-get install pacote
- sudo apt-get upgrade pacote
- sudo apt-get remove pacote

- apt-cache search pacote
  - Obtém informações sobre o pacote

## Extensão .deb

- Instala pacotes do tipo .deb
  - sudo dpkg -i pacote.deb

- Descrição do Pacote
  - sudo dpkg -I pacote.deb

- Remoção
  - sudo dpkg -r nomedopacote

## Extensão .rpm

- Instalação
  - sudo rpm -ivh pacote.rpm

- Atualização
  - sudo rpm -U pacote.rpm

- Remoção
  - sudo rpm -e pacote.rpm

## yum

- Instalação
  - sudo yum install pacote

- Atualização
  - sudo yum update pacote

- Remoção
  - sudo yum remove pacote


## Atualização do Sistema

- sudo apt update && apt upgrade


# sudo

- Elevação de privilégios
