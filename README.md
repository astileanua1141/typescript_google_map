### Description

This repository contains a small TypeScript proof of concept.
The objective is to display a new Google Map in  a browser window, and show 2 randomly generated location coordinates, for a User and a company. Clicking on them will show a description pop-up window, displaying random generated names or, for companies, the catchphrase. 

This project has a learning objective through practice. <br/>
- This is the 2<sup>nd</sup>  app resulted from the "[Apendix B] Basics of Typescript" from <br/>
:school: **Course**: [Udemy - Microservices with Node.JS and React](https://www.udemy.com/course/microservices-with-node-js-and-react/) <br/>

- The first app is in this repository: https://github.com/astileanua1141/service_bus_kubernetes_mvp
<br/>

### Installation

- remember to replace the <API-key> with the actual key, in index.html
- to run this project on local dev machine (instead of nodemon + ts support): 

  `$ npm install -g parcel-bundler ` <br/>
  `$ parcel index.html`

### Dependencies: 
  - @faker-js/faker (v7.5.0) to generate random names, coordinates and catchphrases
  - @types/google.maps (v3.50.2) used to display and manage the Map
   

### TODOs:
  - [FIXME] In ***CustomMaps.ts***, the constructor for a new Map requires a non-null HTML Element. A quick fix was to provide a *size* and *width* in the *style* element, in ***index.html***, so the map display is correct. <br/>
  Reference:
    > CustomMaps.ts: <br/>
    > `new google.maps.Map(document.getElementById(divId)...` 
  - [best practice] Introduce the API key as an environment constant, but the project is really small so I skipped that for now 