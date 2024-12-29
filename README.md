# Node_and_Angular_Project

## Team Members
- Jérémie FORMEY DE SAINT LOUVENT: CDOF2
- Camille DUPRE LA TOUR: CDOF2
- Ryan JABBOUR: CDOF2

This project is a Cinema Booking System built with a Node.js backend and an Angular frontend. The code is written in TypeScript (.ts).

## Project Structure
The project is divided into two main parts:
Frontend: Built using Angular
Backend: Built using Node.js

### Frontend
The frontend provides a user-friendly interface to interact with the cinema booking system. It allows users to view available movies, make reservations, and view their bookings.

Key Features:
- Catalog: Displays a list of available movies.
- Make Reservation: Allows users to select a movie, choose a showtime, and make a reservation.
- Reservations: Shows a list of reservations made by the user.

The frontend is structured as follows:
- Nav Bar: A navigation bar is available for accessing the three pages:
    - Catalog
    - Make Reservation
    - Reservations

Files and Components:
- CatalogComponent (catalog.component.ts, catalog.component.html): Displays the list of available movies using ag-Grid.
- MakeReservationComponent (make-reservation.component.ts, make-reservation.component.html): Provides a form for users to make a reservation.
- ReservationsComponent (reservations.component.ts, reservations.component.html): Displays the user’s reservation history.
- Other important files:
    - app-routing.module.ts: Defines the routes for the application, mapping URLs (e.g., /catalog) to corresponding components.
    - app.module.ts: Main configuration file that imports necessary dependencies, registers components, and initializes the app.
    - app.component.ts: Root component containing the <router-outlet> for rendering components based on routes.

Libraries Used:
- ag-Grid: For displaying the catalog of movies in a grid format.
- Highcharts: For visualizing data, such as booking statistics or movie performance.
- Leaflet: For mapping the cinema locations or showtimes.


### Backend
The backend is built using Node.js and provides the necessary API for managing movies, reservations, and users.

Key Features:
- Admin Functionality: Admins can create new movies via the backend.
- User Functionality: Users can view movies, make reservations, and save them to the database.
- Database: MySQL is used to store all system data. The database is named cinemabookingsystem and contains the following tables:
    - Users Table: Stores user details, including a unique ID, name, email (unique), and phone number.
    - Movies Table: Stores movie information, such as title, genre, release date, and duration.
    - Bookings Table: Tracks user bookings, with references to the user and movie IDs, showtimes, booking date, and the number of tickets.
    - Showtimes Table: Stores movie showtimes, linking to the Movies table to specify when each movie will be shown.
