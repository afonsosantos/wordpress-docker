# wordpress-docker
Wordpress com Docker Compose e SSL

**Artigo de Referência**: [https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-with-docker-compose](https://www.digitalocean.com/community/tutorials/how-to-install-wordpress-with-docker-compose)


## Instalação e Uso

### Passo 1 - Clonar o Repositório

```shell
$ git clone https://github.com/afonsosantos/wordpress-docker.git wp/
$ cd wp/
```

### Passo 1 - Variáveis de Ambiente

Criar o ficheiro `.env` e preencher as variáveis abaixo:

- **MYSQL_ROOT_PASSWORD**=your_root_password
- **MYSQL_USER**=your_wordpress_database_user
- **MYSQL_PASSWORD**=your_wordpress_database_password

### Passo 2 - Instalar Docker e Docker Compose

1. Instalar o **Docker**:

```shell
$ curl -sSL http://get.docker.io | bash
```

2. Instalar o **Docker Compose**:

```shell
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.26.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

*(verificar a versão no comando, e substituir se exitir uma mais recente)*

3. Tornar o binário executável:

```shell
$ sudo chmod +x /usr/local/bin/docker-compose
```

### Passo 3 - Iniciar os Serviços

```shell
$ docker-compose up -d
```
