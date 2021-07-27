# Servidores Físicos

<br>

- Servidores para cada serviço do sistema;
- Gera vários problemas, entre eles o custo de luz e rede, e o seu alto tempo de ociosidade.

<br>

- <b>Solução: Máquinas Virtuais. </b>

<br>

# Máquina Virtuais

<br>

- Virtualização dos recursos físicos;
- Redução do custo de luz e rede e redução da ociosidade.

<br>

- Como as máquinas virtuais possuem sistemas operacionais, os mesmos possuem um custo de hardware para manter suas funcionalidades;
- Como as máquinas virtuais possuem sistemas operacionais, os mesmos possuem configurações iniciais a serem feitas, e devem ser atualizados com frequência;
- Manter vários sistemas operacionais requer muito tempo de trabalho, chegando a equivaler ao tempo requerido para manter as aplicações.

<br>

- <b>Solução: Containers. </b>

<br>

# Containers

<br>

- Melhor controle do uso dos recursos do Sistema Operacional;
- Agilidade na hora de criar e remover aplicações;
- Maior facilidade na hora de trabalhar com diferentes versões de bibliotecas e linguagens.

<br>
<br>
<br>

# Docker

- Uma imagem é formada de uma ou várias camadas READ ONLY;
- Ao criar um container utilizando essa imagem, é criado uma nova camada READ/WRITE;
- Uma imagem pode criar diversos containers.