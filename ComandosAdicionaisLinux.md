## wc

* wc -l [arquivo]: Número de linhas do arquivo
* wc -w [arquivo]: Número de palavras do arquivo
* wc -c [arquivo]: Número de bytes do arquivo
* wc -m [arquivo]: Número de chars do arquivo
- Somente wc:
  - Primeiro número: linhas
  - Segundo número: palavras
  - Terceiro número: bytes

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

- su nome_do_usuário : Troca para este usuário
- useradd -m nome_do_usuário : Adiciona um usuário com o próprio diretório

- Se não possuir permissão, adicionar 'sudo' antes dos comandos: sudo su, sudo adduser

```bash
sudo userdel -r user     # Remove o user e o diretório home
```

### Mudar Senha

```bash
passwd    # Muda a própria senha

sudo passwd user   # Muda a senha do user
```

## ls -lh

- Verifica as permissões do diretório
  - r: read; w: write; x: execution

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

<strong>

- read = 4
  
- write = 2

- execute = 1
  
</strong>

```bash
chmod 200 arquivo   # Somente o dono pode escrever no arquivo
chmod 300 arquivo   # Somente o dono pode escrever e executar (2 + 1) no arquivo
chmod 700 arquivo   # Somente o dono possui todas as permissões
chmod 754 arquivo   # Dono possui todas as permissõs; Grupo pode ler e executar; Outros podem ler

chmod +t diretorio/     # Garante que somente o usuário que criou o arquivo dentro do diretório, consegue deletá-lo
```

### Outro Modo de Dar Permissões

```bash
chmod u+rwx    # Usuário (u: padrão), permissão de escrita, leitura e execução

chmod o-rwx    # Outros (o), tira a permissão de tudo

# Para diretórios

chmod -R o+w Documents
```

## chown

- Muda o dono do arquivo ou diretório.
```bash
sudo chown new_owner arquivo.txt
```

## group

```bash
sudo groupadd novo_grupo

sudo usermod -a -G novo_grupo user    # Adiciona o user ao novo_grupo
```

```bash
id user     # Mostra os grupos do user
```

## read

```bash
read IDADE
22
echo $IDADE
```

