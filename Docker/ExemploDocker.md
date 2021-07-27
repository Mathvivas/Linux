# Dockerfile

<br>
<br>

### Exemplo: Projeto node

<br>

```dockerfile
# Cria a imagem com base em outra
FROM node:latest
MAINTAINER Matheus
# Copia o código do diretório atual para a do volume
COPY . /var/www
# Comandos executados no WORKDIR
WORKDIR /var/www
# Roda o comando ao construir a imagem
RUN npm install
# Ao carregar o container, será executado este comando
# ENTRYPOINT npm start
ENTRYPOINT ["npm", "start"]
# Porta da aplicação
EXPOSE 3000
```