# Project description

Checkino is an application, that will help digital nomads with world trip.

# Required features

- Synchronise my Swarm (Foursquare) check-ins, retrieve it from Foursquare via Personalization API ( https://docs.foursquare.com/developer/reference/personalization-apis-authentication) and store it in local database
- Show a world map with pins on all my checkins
- Have a separate page, that will show a summary by each country with statistics how many days I spend in each country and when. Stays in county will be added manually and store in DB. Also there should be suggestions to add new country travel record, based on data from Foursquare check-ins
- Authorisation to my app must be via Google login

# Technologies

App must have 2 parts:
- checkino-app-service - backend Spring Boot application
- checkino-web - Frontend React app

## checkino-app-service

- Spring Boot Java application
- Reactive - Spring WebFlux
- MongoDB

## checkino-web

- React app
- Build Tool - Vite
- PNPM as a package manager
- Typescript
- Airbnb TS ESLint configs
- MUI Joy as a component library
- Caddy as a prod web server

# Instructions

- Code should follow clean code principles and best practices
- Docker will be used for prod deployment
- To access Foursquare API, user must complete authentication (endpoint is in API doc). This "link" to Foursquare should be stored in someway, so when user login to Checkino app, he don't need to login again in Foursquare
