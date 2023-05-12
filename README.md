# DSList

# Sobre o projeto

DSList é um sistema construído durante uma das edições da **Semana DevSuperior**, evento organizado pela [DevSuperior](https://devsuperior.com.br "Site da DevSuperior").

O sistema consiste em uma coleção de jogos eletrônicos por lista, nesse projeto desenvolvemos somente o back-end da aplicação.

# Passos

- Criar projeto / lib Maven
- Salvar no Github
- Arquivos Properties, entidade Game, ORM
- Seed dos games
- GameMinDTO, GameRepository, 
GameService, GameController

- Implementar modelo de domínio
- Atualizar seed da base de dados
- GameDTO, busca game por id
- Busca totas listas em /lists
- Consulta SQL, projection, busca de games 
por lista

## Passos em homologação

Preparação do ambiente
Docker
ou
Postgresql + pgAdmin ou DBeaver
Homologação local
1. Criar perfis de projeto
* system.properties
2. Gerar script da base de dados
* apagar arquivo gerado
3. Criar base de dados de homologação
4. Rodar app no modo dev e validar

# Passos deploy CI/CD

## Passos Railway
1. Prover um servidor de banco de dados 
2. Criar a base de dados e seed
3. Criar uma aplicação Railway vinculada a um 
repositório Github
4. Configurar variáveis de ambiente
 APP_PROFILE
DB_URL (Formato: 
jdbc:postgresql://host:porta/nomedabase)
DB_USERNAME
DB_PASSWORD
CORS_ORIGINS
 5. Configurar o domínio público para a aplicação
6. Testar app no Postman
7. Testar a esteira de CI/CD

## Modelo de domínio DSList
![Modelo de domínio DSList](https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/dslist-model.png)

# Tecnologias utilizadas
## Back end
- Java
- Spring Boot
- JPA / Hibernate
- Maven

## Implantação em produção
- Back end: Railway
- Banco de dados: Postgresql

# Como executar o projeto

## Back end
Pré-requisitos: Java 17

```bash
# clonar repositório
git clone https://github.com/Nullwell47/dslist.git

# entrar na pasta do projeto back end
cd dslist

# executar o projeto
./mvnw spring-boot:run
```

# Autor

Emanoel Rosa Barros

https://www.linkedin.com/in/emanoel-rosa-323b381a2/

