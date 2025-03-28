# Board

O **Board** é um sistema de gerenciamento de tarefas desenvolvido em Java. Ele permite criar, organizar e gerenciar boards, colunas e cards, com funcionalidades como movimentação de cards entre colunas, bloqueio/desbloqueio de cards e cancelamento de tarefas.

## Funcionalidades

- Criação de boards com colunas personalizadas.
- Gerenciamento de colunas (Inicial, Pendente, Final, Cancelamento).
- Criação, movimentação, bloqueio e desbloqueio de cards.
- Visualização de detalhes de boards, colunas e cards.
- Persistência de dados em banco de dados MySQL.
- Migração de banco de dados utilizando Liquibase.

## Pré-requisitos

Certifique-se de ter os seguintes itens instalados em sua máquina:

- [Java Development Kit (JDK)](https://www.oracle.com/java/technologies/javase-downloads.html) 11 ou superior.
- [Gradle](https://gradle.org/) para gerenciamento de dependências.
- [Docker](https://www.docker.com/) e [Docker Compose](https://docs.docker.com/compose/) para execução do banco de dados.

## Como executar o projeto

### Configuração do Banco de Dados

1. Certifique-se de que o Docker e o Docker Compose estão instalados e em execução.
2. No diretório raiz do projeto, execute o seguinte comando para iniciar o banco de dados MySQL:
   ```bash
   docker-compose up -d
   ```

### Executando o Projeto

1. Clone o repositório:
   ```bash
   git clone https://github.com/iamfernandareis/java-board.git
   cd board
   ```

2. Compile o projeto usando Gradle:
   ```bash
   ./gradlew build
   ```

3. Execute a aplicação:
   ```bash
   java -jar build/libs/Board-1.0-SNAPSHOT.jar
   ```

## Estrutura do Projeto

- `src/main/java`: Código-fonte principal.
- `src/main/resources`: Arquivos de configuração e scripts de migração do banco de dados.
- `src/test/java`: Testes automatizados.
- `docker-compose.yml`: Configuração do banco de dados MySQL.
- `build.gradle.kts`: Configuração do Gradle.

## Tecnologias Utilizadas

- **Java**: Linguagem principal do projeto.
- **Gradle**: Gerenciador de dependências e build.
- **Liquibase**: Controle de versão do banco de dados.
- **MySQL**: Banco de dados relacional.
- **Lombok**: Redução de boilerplate no código Java.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.
