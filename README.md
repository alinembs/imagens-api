# imagens-api

API REST construída com **Spring Boot** (Java 17) para gerenciar recursos relacionados a imagens.

## Tecnologias

- Java 17
- Spring Boot 3.2.2
- Maven
- H2 (configurado como dependência)

## Estrutura do projeto

- `src/main/java/com/alinembs/imageapi/ImageapiApplication.java`
  - Classe principal do Spring Boot.
- `src/main/java/com/alinembs/imageapi/images/ImagensController.java`
  - Controller REST sob o prefixo `/v1/images`.
- `src/main/resources/application.properties`
  - Configurações da aplicação (arquivo presente).

## Endpoints

O controller `ImagensController` está mapeado para:

- Prefixo: `GET/POST/PUT/... /v1/images`

No momento, o controller não possui métodos/rotas ativas além do mapeamento base (há código comentado).

## Como rodar localmente

1. Navegue para a pasta do projeto:
   - `cd ./imagens-api`
2. Suba a aplicação com Maven:
   - `./mvnw spring-boot:run`
3. Acesse a API no servidor local (porta padrão do Spring Boot, se não configurada em `application.properties`).

## Testes

- Teste de contexto:
  - `src/test/java/com/alinembs/imageapi/ImageapiApplicationTests.java`

Para executar:

- `./mvnw test`

## Dependências relevantes (pom.xml)

- `spring-boot-starter-web` (API REST)
- `spring-boot-starter-data-jpa` (persistência via JPA)
- `com.h2database:h2` (banco H2)
- `spring-boot-starter-test`
