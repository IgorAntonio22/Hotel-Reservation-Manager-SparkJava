# Gerenciador De Reservas De Hotel

## Sobre o Projeto

Este projeto é uma aplicação RESTful desenvolvida em Java com o framework Spark, destinada ao gerenciamento de reservas em hotéis. O sistema permite a inserção, exclusão e consulta de hotéis, andares e quartos, bem como a realização de reservas para hóspedes. A aplicação está estruturada em diferentes módulos para gerenciar hotéis, clientes, acomodações e quartos, garantindo uma organização clara e eficiente dos dados.

## Funcionalidades

- **Gerenciamento de Hotéis**: Adicione, remova e consulte hotéis.
- **Gerenciamento de Clientes**: Crie, exclua e consulte informações de clientes.
- **Gerenciamento de Acomodações**: Adicione, remova e consulte andares específicos dentro de um hotel.
- **Gerenciamento de Quartos**: Adicione, remova e consulte quartos específicos dentro de um andar.
- **Reserva de Quartos**: Realize reservas para hóspedes em quartos específicos de um hotel.

## Endpoints

### Hotéis
- `GET /hoteis`: Retorna a lista de hotéis.
- `POST /hoteis`: Adiciona um novo hotel.
- `DELETE /hoteis/:id`: Remove um hotel pelo ID.
- `GET /hoteis/:id`: Retorna um hotel pelo ID.

### Clientes
- `GET /clientes`: Retorna a lista de clientes.
- `POST /clientes`: Cria um novo cliente.
- `DELETE /clientes/:id`: Remove um cliente pelo ID.
- `GET /clientes/:id`: Retorna um cliente pelo ID.

### Reservas
- `POST /:id/reservar`: Realiza uma reserva para um cliente em um quarto específico.

### Acomodações
- `GET /acomodacoes/:idDoHotel`: Retorna a lista de acomodações (andares) de um hotel específico.
- `POST /acomodacoes/:idDoHotel/:idDaAcomodacao`: Adiciona uma nova acomodação (andar) em um hotel específico.
- `DELETE /acomodacoes/:idDoHotel/:idDaAcomodacao`: Remove uma acomodação (andar) pelo ID no hotel específico.
- `GET /acomodacoes/:idDoHotel/:idDaAcomodacao`: Retorna uma acomodação (andar) pelo ID no hotel específico.

### Quartos
- `GET /quartos/:idDoHotel/:idDaAcomodacao`: Retorna a lista de quartos em uma acomodação (andar) específica de um hotel.
- `POST /quartos/:idDoHotel/:idDaAcomodacao`: Adiciona um novo quarto em uma acomodação (andar) específica de um hotel.
- `DELETE /quartos/:idDoHotel/:idDaAcomodacao/:idDoQuarto`: Remove um quarto pelo ID em uma acomodação (andar) específica de um hotel.
- `GET /quartos/:idDoHotel/:idDaAcomodacao/:idDoQuarto`: Retorna um quarto pelo ID em uma acomodação (andar) específica de um hotel.

## Como Executar

1. **Pré-requisitos**: Certifique-se de ter o Java instalado em sua máquina.
2. **Clonar o Repositório**: `git clone <URL-do-repositório>`
3. **Construir o Projeto**: Utilize o Maven para construir o projeto. Execute `mvn clean install` na raiz do projeto.
4. **Executar a Aplicação**: Execute a aplicação através da classe principal.

