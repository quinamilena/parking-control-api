# Parking Control

Api em Spring Boot para cadastro de carros em vagas de estacionamento.

# Instação

- Java Jdk
- Maven
- Docker desktop
- IDE para Spring Boot

# Como usar

- Na pasta raiz `docker compose up -d`, para iniciar os serviços dos Postgres e PDAdmin;
- Abrir o `PDAdim` no link `http://localhost:5050/`;
- Ir em Servers > Create > Server, dá um nome para a conexão.
  - Para descobrir o host é preciso fazer:
    - `docker ps` para listar os containers ativos;
    - Selecionar o id do container da image postgres;
    - Inspecionar o container, `docker inspect id_container`;
    - Selecionar o ip da propriedade `Gateway`;
  - A senha é admin e salvar;
- Depois é preciso dá o start da aplicação;
- Após usar aplicação parar o container `docker compose down`;
