# Description

Information related to HTTP calls from server or client side.

## HTTP Call Approaches

1. In Node
   1. http
      1. directly in node
   2. request
      1. higher-level library that is popular
2. In Browser
   1. XMLHttpRequest
      1. Old - from 1999!!
      2. A lot of boilerplate code to work!
   2. jQuery
      1. $.ajax object
      2. Makes sense if you are using jQuery already (eliminates dependencies)
   3. Framework-based
      1. i.e. Angular has it's own built-in http service
   4. Fetch
      1. Popular library
      2. Still in infancy as of 2014 - need polyfills for unsupported browsers
   5. Node & Browser
      1. "Universal JavaScript" if it support both client and browser
      2. isomorphic-fetch
         1. fetch-like api (npm package)
      3. xhr
         1. npm package - subset of node/request library
      4. SuperAgent
         1. Full-featured
         2. Node.js and browser
      5. Axios
         1. Full-featured
         2. Node.js and browser
         3. Clean, promise-based API

## Centralizing API Calls

Why?

1. Configure all calls
2. Handle preloader logic centrally
3. Handle errors centrally
4. Single interface for mocking http requests

## For this course

1. We will use fetch (we are browser-side only)
2. We will centralize our API calls

# How to Mock HTTP

1. Nock
   1. Intercepts requests and sends static responses
2. Static JSON
   1. Same JSON every time
3. JSON Server
   1.  Saves updates to the data
4. JSON Server + JSON Schema Faker
5. Full Server - Express, etc.

## Our plan for mocking http

1. Declare our schema
   1. JSON Schema Faker
      1. Comes bundled with faker.js, Chance, and randexp.js
2. Generate Random Data:
   1. faker.js
      1. https://github.com/Marak/faker.js/wiki
      2. https://marak.github.io/faker.js/index.html
   2. chance.js
   3. randexp.js
3. Serve Data via API
   1. JSON Server

