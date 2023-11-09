# Railway-System-Database

This repository contains a database project for managing railway system information, including stations, timetable, passengers, fare schedules, and tickets.

## Database Structure

### 1. Station Table
- Manages information about railway stations, including StationId and StationName.
- Includes sample data for various stations.

### 2. Timetable Table
- Stores timetable details, including timeTable, StationId, departureTime, and arrivalTime.
- Default constraint is set for StationID.

### 3. Passenger Table
- Records information about passengers, including passengerId, passengerName, passengerGender, passengerAge, passengerEmail, passengerNumber, and Adres.
- Includes a check constraint for ensuring the passenger age is greater than 0.
- Sample data for passengers with their addresses.

### 4. Fare Schedules Table
- Manages fare schedules, including fareId, timeTable, StationId, SingleFare, and ReturnFare.
- Foreign key references to timetable and Station tables.

### 5. Ticket Table
- Handles ticket information, including ticketId, passengerId, fromStationName, toStationName, dateIssued, single_or_return, fare, and fareId.
- Triggers for insert, delete, and update operations, showing the affected rows.

## Queries and Views

### Sample Queries
- Inner join and order stations with fare schedules.
- Left join stations with fare schedules.
- Selecting information from the timetable.

### Sample Views
- Displaying passenger details along with their ticket information.
- Executing a stored procedure to view passenger details based on name and age.

## Usage
1. Execute the SQL script to create the database and tables.
2. Run the provided queries to retrieve information about stations, timetable, passengers, fare schedules, and tickets.
3. Utilize the views for comprehensive data analysis.
4. Explore stored procedures for specific queries.
