# Docker: metabase-postgres

Criar image docker do metabase integrado com postgres

### 📋 Pré-requisitos

* Ambiente Linux - Ubuntu 20.04
* Docker

### 🔧 Instalar Docker Compose

Para instalar docker-compose, é necessário atualizar lista de pacotes no terminal Linux.

```
sudo apt update
```

Em seguida execute:
```
sudo apt install docker-compose
```

Para confirmar a instalação do docker-compose, execute o seguinte comando:
```
docker-compose --version
```

## ⚙️ Executando os Metabase com Docker Compose

Após baixar o projeto, acesse o diretorio git do projeto
Execute o comando abaixo:
```
docker-compose up -d
```

## 📦 Iniciando a Imagem

Para acessar a imagem criada, execute o seguinte comando:
```
docker-compose up
```

## 🛠️ Configuração

Para acessar a base de dados do PostgreSql 
```
 HOST_NAME: docker_postgres
 PORT: 5433
 DATABASE: metabase
```
É necessário criar o usuário:
```
 USER: metabase
 PASSWORD: postgres
```

## 🖇️ No browser

Digite: http://localhost:3001
Faça o seu cadastro no ambiente do METABASE

Para adicionar um database para PRODUÇÃO
```
 HOST_NAME: docker_postgres
 PORT: 5432
 USER: metabase
 PASSWORD: postgres
```
