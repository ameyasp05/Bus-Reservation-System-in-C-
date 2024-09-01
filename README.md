## Bus Reservation System

### Overview
This project implements a basic bus reservation system in C, allowing users to view available buses, book tickets, cancel bookings, and check the status of a bus. The system manages up to 5 buses, each with 32 seats.

### Features
1. **Login System**: Users must log in with a predefined username and password to access the system.
2. **View Bus List**: Displays a list of available buses.
3. **Book Tickets**: Allows users to book seats on a specific bus. The system tracks the availability of seats and calculates the total booking amount.
4. **Cancel Booking**: Users can cancel a previously booked seat, and the seat becomes available again. The cancellation returns a predefined amount.
5. **Bus Status Board**: Shows the seating arrangement of a selected bus, indicating which seats are occupied and by whom.

### Code Structure
- **Main Function**: Handles the user interface, presenting a menu for various operations and executing the corresponding functions based on user input.
- **bus()**: Displays the list of buses.
- **booking()**: Manages ticket booking, updates the seat availability, and records passenger details.
- **name_number()**: Stores the passenger's name and seat number in the corresponding files.
- **read_number()**: Reads seat numbers from a file and populates them into an array.
- **read_name()**: Reads passenger names from a file and stores them in an array.
- **status()**: Displays the current status of seats in a specific bus.
- **status_1()**: Helper function for displaying seat status during booking and cancellation.
- **cancle()**: Allows the user to cancel a booked seat and updates the seat status.
- **login()**: Implements a basic login mechanism with predefined credentials.

### Files Used
- **tr1.txt, tr2.txt, ... tr5.txt**: Files used to store seat availability for each bus.
- **status1.txt, status2.txt, ... status5.txt**: Files used to store the names of passengers for each bus.
- **number1.txt, number2.txt, ... number5.txt**: Files used to store seat numbers for each bus.

### How to Use
1. **Login**: Start the program, enter the username (`user`) and password (`pass`) to log in.
2. **View Bus List**: Choose option `1` from the menu to see the list of available buses.
3. **Book Tickets**: Choose option `2`, select a bus, enter the number of tickets, and provide passenger details.
4. **Cancel Booking**: Choose option `3`, select the bus, and enter the seat number to cancel.
5. **Bus Status Board**: Choose option `4` to view the seating arrangement of a bus.

### Notes
- The system uses text files to persist seat availability and passenger data.
- Make sure to have the required text files (`tr1.txt` to `tr5.txt`, etc.) in the same directory as the executable. Each should start with "32" (indicating all seats are available).
- The code includes a simple login system; you can modify the username and password in the `login()` function.
