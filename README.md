# HotelReservationManager

## About the Project

This project is a RESTful application developed in Java using the Spark framework, designed for managing hotel reservations. The system allows for the insertion, deletion, and querying of hotels, floors, and rooms, as well as making reservations for guests. The application is structured into different modules to manage hotels, clients, accommodations, and rooms, ensuring a clear and efficient organization of data.

## Features

- **Hotel Management**: Add, remove, and query hotels.
- **Client Management**: Create, delete, and query client information.
- **Accommodation Management**: Add, remove, and query specific floors within a hotel.
- **Room Management**: Add, remove, and query specific rooms within a floor.
- **Room Reservation**: Make reservations for guests in specific hotel rooms.

## Endpoints

### Hotels
- `GET /hoteis`: Returns the list of hotels.
- `POST /hoteis`: Adds a new hotel.
- `DELETE /hoteis/:id`: Removes a hotel by ID.
- `GET /hoteis/:id`: Returns a hotel by ID.

### Clients
- `GET /clientes`: Returns the list of clients.
- `POST /clientes`: Creates a new client.
- `DELETE /clientes/:id`: Removes a client by ID.
- `GET /clientes/:id`: Returns a client by ID.

### Reservations
- `POST /:id/reservar`: Makes a reservation for a client in a specific room.

### Accommodations
- `GET /acomodacoes/:idDoHotel`: Returns the list of accommodations (floors) in a specific hotel.
- `POST /acomodacoes/:idDoHotel/:idDaAcomodacao`: Adds a new accommodation (floor) in a specific hotel.
- `DELETE /acomodacoes/:idDoHotel/:idDaAcomodacao`: Removes an accommodation (floor) by ID in a specific hotel.
- `GET /acomodacoes/:idDoHotel/:idDaAcomodacao`: Returns an accommodation (floor) by ID in a specific hotel.

### Rooms
- `GET /quartos/:idDoHotel/:idDaAcomodacao`: Returns the list of rooms in a specific accommodation (floor) of a hotel.
- `POST /quartos/:idDoHotel/:idDaAcomodacao`: Adds a new room in a specific accommodation (floor) of a hotel.
- `DELETE /quartos/:idDoHotel/:idDaAcomodacao/:idDoQuarto`: Removes a room by ID in a specific accommodation (floor) of a hotel.
- `GET /quartos/:idDoHotel/:idDaAcomodacao/:idDoQuarto`: Returns a room by ID in a specific accommodation (floor) of a hotel.

## How to Run

1. **Prerequisites**: Ensure you have Java installed on your machine.
2. **Clone the Repository**: `git clone <repository-url>`
3. **Build the Project**: Use Maven to build the project. Run `mvn clean install` in the project root directory.
4. **Run the Application**: Run the application through the main class.


