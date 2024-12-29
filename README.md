# Node_and_React_Project

# Team Members : 
Jérémie FORMEY DE SAINT LOUVENT, CDOF2
Camille DUPRE LA TOUR, CDOF2
Ryan JABBOUR, CDOF2

This project is a Cinema booking system.

The code is divided into two parts : project-frontend and backend.

The frontend is made using Angular. The backend is made using Node. 

The code is in typescript (.ts).

The frontend is displaying the movies available, the reservation menu, and the bookings made for a given cinema session.
The menu of the frontend contains a nav bar. 
The frontend contains 3 pages accessible from the nav bar. Corresponding to its 3 components : 
- catalog
- make-reservation
- reservations
  
Each of them contains a .ts file and .html file. 
It also contains :
- The app-routing.module.ts file defines the routes for the application, mapping URLs like /catalog to specific components such as CatalogComponent. It uses Angular's RouterModule to handle navigation within the app
- The app.module.ts file is the main configuration file, where all components, modules, and services are registered. It ensures the application is properly initialized by importing necessary dependencies
- The app.component.ts file defines the root component of the app, serving as the main container for the app’s content. It includes the <router-outlet> in its template to display components based on the current route


Backend :
- The backend allows to create a movie (if admin), or to get a movie. 
- It also allow to create a reservation and to input on the sql file storing all of them.
  

