# Flytbase
The project involves designing a system for a big corporation to survey/map its campuses/sites using drones. The system allows users to manage multiple drones assigned to specific campuses/sites and create missions assigned to those sites. The missions can be categorized into path, grid/survey, and corridor types. The system also allows users to manage sites, drones, and missions through backend CRUD services, and shift drones from one site to another. It also includes the ability to manage custom categories, associate them with missions, and retrieve missions/drones by category. The system uses JWT for API authentication and MongoDB to save and retrieve user data.
Backend for flytbase app made using node.js, Express framework

## Installation
Follow the below steps to run the app:-

1. Clone the repo in your local env
2. Set the environment variables present in .env file accordingly
3. Run docker-compose up

This will bind the port(3000) to the host network and start the server on this port.

## Usage
flytbase.postman_collection.json contains collection of API's, header and body.

Follow the below steps to see the working of api's:-

1. Register a user using name, password, email_id.
2. Login using the email_id and password to get the auth token.
3. Pass this auth token in all the further operations with the header property x-auth-token.
3. Register a new site with values (site_name, position). 
4. Register a new drone with values (drone_id, drone_type, make_name, name). 
5. Register a new mission with values (alt, speed, name, waypoints, site).
6. Register a new categorie with values (name, color, tag_name).
7. Assign a drone to the site.
8. Assign a drone to the mission.
9. Assing a category to the mission.
10. Get all missions present in a site.
11. Get all drones present in a site.
12. Get all missions present in a categorie.
13. Get all drones in a categorie.
