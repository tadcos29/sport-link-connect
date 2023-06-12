# Sport-Link-Connect

## Description

A proof-of-concept mock-up of a web application aiming to connect individual outdoorspeople on the basis of geographical points of common interest.

## Introduction and Purpose:

This was my first group project at the coding bootcamp, and the challenge lay in collaboration itself as much, if not more, as in the composition of the application. At the end of the day, the application does not serve a discrete purpose for the visiting user, unless that purpose is simply the display and favouriting of landmarks around the geographical coordinates of the user (if permitted) and having that information persist in local storage. It requires a more mature deployment environment, with some backend support, and of course a great deal of additional work, to actually realise its potential.

Still, it represents my first steps in tackling the challenge of asynchronicity in JavaScript and in shaping fetch requests. The idea of membership and social connection is represented via simulated plain-text-passworded 'accounts' in the browser's local storage, which are able to 'see' each other's favourited landmarks. 

My own responsibilities centered on integrating overall application logic, OpenStreetMap/Nominatim API requests, local storage handling, and the event layer under the user interface masterfully styled by Mario Repas ([Tegrty](https://github.com/Tegrty)). Vasily Likhovaydo ([vasilyl1](https://github.com/vasilyl1)) researched and implemented the core GeoNames API, performed countless instances of heroic troubleshooting, and kept a much-needed eye on the project's pace and scope.

## Technical Overview:

The application fetches geographical landmark information from the GeoNames API and graphical tile data from OpenStreetMap API, leaning on the Leaflet.js library. It combines the two to offer a visual representation of nearby points of interest. It also updates the geographical area under scrutiny on request, by fetching a geocode resolution of a natural-language street address or other location name from the Nominatim API.

Its object structure is intended to be adaptable to the Strava API, once the CORS issues associated with it are overcome, at which point it will cleave closer to its concept, and aim to serve urban fitness enthusiasts in addition to people interested in parks, beaches, kayak portages, and so on.

Its user interface is powered by the Tailwind framework in addition to Bootstrap. 

## Results:

![image](./assets/img/Readme-gif.gif/)


The application is currently live on [GitHub Pages](https://tegrty.github.io/Sport-Link-Connect/) courtesy of Mario Repas.

My GitHub repository for the project is: https://github.com/tadcos29/sport-link-connect
