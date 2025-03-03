# Hotel_Resevation

# HotelReservation - A Java project for hotel reservation management

This is a `java` application for booking hotel rooms .
The goal was to create a hotel application which allows users to book and manage room reservations.

## User Scenarios
The application provides four user scenarios:

1. <b>Creating a customer account</b>: The user needs to first create a customer account before they can create a reservation.

2. <b>Searching for rooms</b>: The app should allow the user to search for available rooms based on provided checkin and checkout dates. If the application has available rooms for the specified date range, a list of the corresponding rooms will be displayed to the user for choosing.

3. <b>Booking a room</b>: Once the user has chosen a room, the app will allow them to book the room and create a reservation.

4. <b>Viewing reservations</b>: After booking a room, the app allows customers to view a list of all their reservations.

## Admin Scenarios
The application provides four administrative scenarios:

1. <b>Displaying all customers accounts</b>.
2. <b>Viewing all of the rooms in the hotel</b>.
3. <b>Viewing all of the hotel reservations</b>.
4. <b>Adding a room to the hotel application</b>.

## Reserving a Room
The application allows customers to reserve a room. Here are the specifics:

1. <b>Avoid conflicting reservations</b>: A single room may only be reserved by a single customer per a checkin and checkout date range.
2. <b>Search for recommended rooms</b>: If there are no available rooms for the customer's date range, a search will be performed that displays recommended rooms on alternative dates. The recommended room search will add seven days to the original checkin and checkout dates to see if the hotel has any availabilities, and then display the recommended rooms/dates to the customer.
> Example: If the customers date range search is 1/1/2025 – 1/5/2025 and all rooms are booked, the system will search again for recommended rooms using the date range 1/8/2025 - 1/12/2025. If there are no recommended rooms, the system will not return any rooms.

### Room Requirements
<b>Room cost</b>: Rooms will contain a price per night. When displaying rooms, paid rooms will display the price per night and free rooms will display "Free" or have a $0 price.
<b>Unique room numbers</b>: Each room will have a unique room number, meaning that no two rooms can have the same room number.
<b>Room type</b>: Rooms can be either single occupant or double occupant (Enumeration: SINGLE, DOUBLE).

### Customer Requirements
The application will have customer accounts. Each account has:

1. <b>A unique email for the customer</b>: RegEx is used to check that the email is in the correct format (i.e., name@domain.com).
2. <b>A first name and last name</b>.
3. The email RegEx is simple for the purpose of this exercise and may not cover all real-world valid emails. 

