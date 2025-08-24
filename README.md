# Hotel Reservation System

A Java-based command-line application for managing hotel room reservations. This system allows users to search for available rooms, make reservations, cancel reservations, and process payments.

## Features

- **Room Management**
  - Multiple room types (Standard, Deluxe, Suite)
  - View available rooms based on date range
  - Room details including pricing and maximum occupancy

- **Reservation System**
  - Book rooms with guest information
  - View reservation details
  - Cancel existing reservations
  - Process payments

- **Data Persistence**
  - Automatic saving of all data to disk
  - Data is loaded automatically when the application starts

## Prerequisites

- Java 17 or higher
- Maven 3.6.0 or higher

## Installation

1. Clone the repository:
   ```bash
   git clone <https://github.com/Ayush-Jack/CodeAlpha_HotelReservationSystem.git>
   cd hotel-reservation-system
   ```

2. Build the project:
   ```bash
   mvn clean package
   ```

## Running the Application

After building the project, you can run the application using:

```bash
java -jar target/hotel-reservation-system-1.0-SNAPSHOT-jar-with-dependencies.jar
```

Or run directly with Maven:

```bash
mvn exec:java -Dexec.mainClass="com.hotel.HotelReservationApp"
```

## Usage

1. **Search & Book a Room**
   - Select room type and date range
   - Choose from available rooms
   - Enter guest information
   - Confirm booking

2. **View Reservation**
   - Enter reservation ID to view details

3. **Cancel Reservation**
   - Cancel an existing reservation using the reservation ID

4. **Process Payment**
   - Mark a reservation as paid using the reservation ID

## Project Structure

```
src/main/java/com/hotel/
├── HotelReservationApp.java      # Main application class
├── model/
│   ├── Room.java                # Room entity class
│   └── Reservation.java         # Reservation entity class
└── service/
    └── HotelService.java        # Core business logic
```

## Testing

Run the test suite with:

```bash
mvn test
```

## Built With

- Java 17
- Maven - Dependency Management
- JUnit 5 - Testing framework

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Future Enhancements

- Add a graphical user interface (GUI)
- Implement user authentication
- Add more room types and amenities
- Generate reports and analytics
- Add support for multiple hotels
