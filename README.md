# G-Events and Maps api

```
npm install
npm run dev
```
### events endpoint:

events from db

[localhost:3000/events](localhost:3000/events)

----

events from galvanize.com scraper

[localhost:3000/events/add](localhost:3000/events/add)

----

#### rooms endpoint:

[localhost:3000/maps](localhost:3000/rooms)

----

### CRUD routes /events

#### CREATE - add new events

/events  method:POST

(expects an object without id)

----

#### READ - read events

/events/:id  method:GET

----

#### UPDATE - update event

/events/:id  method:PUT

(expects an object with id)

----

#### DELETE - delete event

/events/:id   method:DELETE

----

### CRUD routes /rooms

#### CREATE - add new rooms

/rooms  method:POST

(expects an object without id)

----

### READ - read rooms

/rooms/:id  method:GET

----

### UPDATE - update room

/rooms/:id  method:PUT

(expects an object with id)

----

### DELETE - delete room

/rooms/:id   method:DELETE

----

# server scope:

## phase one

create express api endpoint

-   [x] build scraper
-   [x] scrape events data
-   [x] create api end point
-   [x] return events data as json
-   [x] deploy

## phase two

-   [x] discuss /maps response structure so we can build the db to reflect this structure.
-   [x] create db gevents
-   [x] create events migration and test seed(so we start with data in the db),
-   [x] create rooms migration and seed.
-   [x] create CRUD routes and queries for /events and /rooms.
-   [x] change events route to /events
-   [ ] sync the scraped data

## front-end coordination

-   [x] build maps component and link to /maps route
  -   [x] build map with image component
  -   [ ] build floors component (LL, L3, L4 selectors)
  -   [ ] build rooms component (dropdown list)
    * logic: will change the image to selected floor or room.
