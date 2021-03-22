## Rede Wan

- Wide Area Network ou World Area Network é uma rede geograficamente distribuída.

## Rede Man

- Metropolitan Area Network é uma rede metropolitana que interliga várias redes locais.

## Rede Lan

- Local Area Network é uma rede local de uma forma geral em um único prédio ou campus.

## Protocolos

- São as linguagens usadas pelos dispositivos de uma rede de modo que eles consigam se entender.

### IP (Protocolo de Internet)
- Endereço IP: Números que identificam seu computador em uma rede;s
  - IPv4 : 32 bits, série de 4 números de 8 bits -> até 255;
  - IPv6 : Mais endereços (128 bits). 8 conjuntos de 4 dígitos hexadecimais.
- Os IPs normalmente são distribuídos de forma dinâmica, e quem é responsável por isso é o servidor DHCP;
- O equipamento que normalmente temos em casa e que costumamos chamar de roteador, possui um servidor DHCP.

### ICMP (Internet Control Message Protocol) 
- Tem por objetivo prover mensagens de controle na comunicação
entre nós.

- DNS (Domain Name Server): Esse protocolo de aplicação tem por função identificar endereços IPs e manter 
uma tabela com os endereços dos caminhos de algumas redes. Dá nome aos IPs (transforma em sites).
    - Ex: Transforma 216.58.202.132 em www.google.com

## Interface de Rede

- Interface de rede é um software e/ou hardware que faz a comunicação em uma rede de computadores.

-  As interfaces de rede no Linux estão localizadas no diretório /dev e a maioria é criada dinamicamente
pelos softwares quando são requisitadas.

-  A interface loopback é um tipo especial de interface que permite fazer conexões com você mesmo, com ela, 
você pode testar vários programas de rede sem interferir em sua rede padrão. O endereço IP 127.0.0.1 foi 
escolhido para loopback.

## Máscara de Rede

- Determina quais são os IPs da rede;
- Ex : 255.255.255.0, determina que os primeiros 3 números não mudam, somente o quarto varia na rede;
- Em uma rede, todos os IPs terão os mesmos 3 números, somente o quarto será diferente.

## DNS

- Domain Name Service;
- Transforma o nome (site) no seu número correspondente para acesso;
- Sistema hierárquico que associa um IP a um domínio, para que seja possível lembrar de uma forma fácil um site.

# Comandos

### hostname

- Nome do computador na rede.

### hostname -I

- Endereço IP

### ping

- Verifica se o host está ativo ou inativo. Faz parte do Protocolo ICMP.
  - ping www.google.com -w 4 : Envia 4 pacotes

### dig

- Traz informações sobre DNS
  - dig www.google.com
  - dig www.google.com +short : Traz somente o IP

### whois

- whois site : Traz informações do site

### traceroute

- Exibe informações sobre a rota da sua rede até o host desejado
  - traceroute www.google.com

