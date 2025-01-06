Mapty - Workout Tracking Application

Overview
Mapty is an interactive web application that allows users to track their workouts by placing them on a map. Users can log different types of workouts (running and cycling) at specific locations and keep track of various metrics for each workout.
Features

Map Integration: Uses the Leaflet library to display an interactive map
Geolocation: Automatically detects user's location to center the map
Workout Logging:

Running workouts (distance, duration, cadence)
Cycling workouts (distance, duration, elevation gain)


Workout Visualization:

Display workouts on the map with custom markers
Show workout details in a list format


Data Persistence: Stores workout data in local storage
Workout Navigation: Click on a workout to center the map on its location

Technical Architecture
The application follows an object-oriented architecture with the following main components:
Classes

Workout: Base class for workout data
Running: Extends Workout with running-specific calculations
Cycling: Extends Workout with cycling-specific calculations
App: Main application class handling the UI and business logic

Data Flow

Page loads and requests user's current location
Map renders centered on user's location
Previously saved workouts load from local storage
User can:

Click on map to add new workout
Submit workout details via form
Click existing workouts to pan map
View all workouts in sidebar



Technologies Used

HTML5
CSS3 with custom properties (variables)
Modern JavaScript (ES6+)
Leaflet.js for map functionality
Local Storage API for data persistence
Geolocation API

Setup and Installation

Clone the repository
Open index.html in a modern web browser
Allow location access when prompted

Browser Support
The application requires a modern browser with support for:

ES6+ features
Geolocation API
Local Storage
CSS Grid and Flexbox

Usage

Allow location access when prompted
Click anywhere on the map to add a new workout
Fill in the workout details:

Choose workout type (running/cycling)
Enter distance (in km)
Enter duration (in minutes)
Enter cadence (for running) or elevation gain (for cycling)


Press enter or click OK to save the workout
Click on any workout in the list to center the map on that location

Project Structure
Copymapty/
├── index.html          # Main HTML file
├── style.css          # Styles
├── script.js          # Main JavaScript file
├── logo.png           # Application logo
└── README.md          # Documentation
CSS Architecture
The application uses a custom CSS architecture with:

CSS variables for consistent theming
Responsive design using Flexbox and Grid
Custom styling for map markers and popups
Mobile-friendly layout

JavaScript Features

ES6 Classes
Private class fields and methods
Local Storage API
Geolocation API
Event handling
DOM manipulation
Object-oriented programming
Inheritance

Future Enhancements
Potential features that could be added:

Ability to edit workouts
Ability to delete workouts
Ability to delete all workouts
Ability to sort workouts by certain fields
More realistic error messages
Ability to position the map to show all workouts
Ability to draw lines and shapes instead of just points
Geocoding location from coordinates
Display weather data for workout time and place

License
This project is available for use under the MIT License.
