# Holiday Road Redwood Forest
•	The project was intended towards building a web application that allows a user to plan a trip that consists of a National Park, a bizarrerie, and an eatery.
•	In the application, when the user selects a state, we call the National Parks Services API to populate a dropdown of parks, and when they select a park, we use the Open Weather API to generate a 5 day weather forecast which allows the user to see how the weather would be in the near-future at the park they choose. We also used third party APIs to populate the dropdowns for bizarreries and eateries. Once the dropdowns are populated with the data from the APIs the user can select options from each dropdown and details of all three selections will be displayed on the main page. Once a user has selected all three options, they can save their trip to a local database using JSON-Server and view their saved trips in the aside bar.
•	The user can also search for national parks, bizarreries and eateries in the search box provided and related information will be displayed in a dialog box.

![image](https://user-images.githubusercontent.com/8440950/163402192-8a7a3f1d-246a-4e45-80ae-ef86d799b453.png)


## National Park Service API

* API home: https://www.nps.gov/subjects/digital/nps-data-api.htm
* API documentation: https://www.nps.gov/subjects/developer/api-documentation.htm

## Weather API

https://openweathermap.org/api

## Bizarre Destination

http://holidayroad.nss.team/bizarreries

## Eateries Destination

http://holidayroad.nss.team/eateries

## Graphhopper API

1. Register at https://graphhopper.com/dashboard/#/register
1. Once you are authenticated, visit your dashboard at https://graphhopper.com/dashboard/#/overview
1. Request an API key at https://graphhopper.com/dashboard/#/api-keys

### Get Coordinates of Place

#### Request

https://graphhopper.com/api/1/geocode?q=yosemite+national+park&locale=us&debug=true&key=your_api_key

### Get Directions

Once you have the coordinate of a place, you can get directions to it. The first `point` query parameter below is the origin, and the last is the destination. If you have more than waypoint along the way, keep adding points, but always make sure origin is first and destination is last.

https://graphhopper.com/api/1/route?point=starting_latitude,starting_longitude&point=destination_latitude,destination_longitude&vehicle=car&locale=us&instructions=true&calc_points=true&key=your_api_key"


Team members:
- Jordan Andershock
- Eric Bierschenk
- Punam Ahire

Wireframe:
Figma: https://www.figma.com/file/wS4AJT4OGLBmqQmCCdopKJ/Untitled?node-id=2%3A2

ERD:
![Alt text](ERD-holiday-trip.png "Title")
