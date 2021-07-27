# run

- Procura a imagem localmente, caso não encontre, puxa da nuvem.

```bash
docker run ${imagem}
```

- Atrela o terminal do ubuntu com o pc do usuário.

```bash
docker run -it ubuntu
```

- Para baixar imagens não oficiais

```bash
docker run ${usuarioDono}/${imagem}
```

<br>

# ps

```bash
# Exibe os containers que estão rodando
docker ps

# Exibe todos os containers
docker ps -a
```

# start

- Inicializa o container já existente.

```bash
docker start ${containerID}
```

# stop

```bash
docker stop ${containerID}
```

# rm

```bash
docker rm ${containerID}
```

- Remove todos os containers inativos.

```bash
docker container prune
```

# images

```bash
docker images
```

- Remover imagens

```bash
docker rmi ${imagem}
```

# Ports

- Roda o container não atrelado ao terminal (-d) (background) e define uma porta para o site (-P).

```bash
docker run -d -P ${imagem}
```

- Para checar as portas dos containers.

```bash
docker ps

# OU

docker port ${containerID}
```

- Definir uma porta

```bash
docker run -d -p 12345:80 ${imagem}
```

# Nomes do Container

- Não será necessário referenciá-lo pelo id.

```bash
docker run -d -P --name meu-site ${imagem}
```

# Persistência de Dados (Volumes)

- Especificar um caminho no container que grave em uma pasta do próprio computador;
- Tudo o que for escrito no caminho /var/www do container, será na verdade escrito no caminho indicado pelo usuario no próprio computador.

```bash
docker run -v "${caminhoDiretorioUsuario}:/var/www" ${imagem}

# Podem ser dados certos comandos, Ex: Node
docker run -p 8080:3000 -v "${caminhoDiretorioUsuario}:/var/www" -w "/var/www" node npm start
```

# build

- Constrói a imagem a partir do arquivo Dockerfile.

```bash
docker build -f ${nomeDoArquivoDocker} -t ${usuario}/${nomeDaImagem} ${diretorioDoArquivo}
```