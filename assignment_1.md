# Hotel Reservation Booking App

We are going to build a RESTful api for a hotel booking application.
## Assignment 1
For the first assignment you will have to create endpoints to manage hotel room and hotel guests. We can create and retrieve hotel rooms and hotel guests.
Those data will be saved into a database. 
 
### Here are the 3 endpoints for the room resource
GET:  /api/room
```json
{
  "rooms:" [
    {
      "id": "947af28f-6c93-4225-8eed-e1c72c1f722e",
      "nr": 101,
      "description": "A beautifull room with a single king size bed"
    },
    {
      "id": "8130d1bd-a01e-43dd-88b3-3d24fd472c3c",
      "nr": 203,
      "description": "A corner room with two single beds including a small kitchen"
    }
  ]
}
```
GET:  /api/room/{id}
# Hotel Reservation Booking App

We are going to build a RESTful api for a hotel booking application.
## Assignment 1
For the first assignment you will have to create endpoints to manage hotel room and hotel guests. We can create and retrieve hotel rooms and hotel guests.
Those data will be saved into a database. 
 
### Here are the 3 endpoints for the room resource
GET:  /api/room
```json
{
  "rooms:" [
    {
      "id": "947af28f-6c93-4225-8eed-e1c72c1f722e",
      "nr": 101,
      "description": "A beautifull room with a single king size bed"
    },
    {
      "id": "8130d1bd-a01e-43dd-88b3-3d24fd472c3c",
      "nr": 203,
      "description": "A corner room with two single beds including a small kitchen"
    }
  ]
}
```
GET:  /api/room/{id}

```json
{
  "id": "8130d1bd-a01e-43dd-88b3-3d24fd472c3c",
  "nr": 203,
  "description": "A corner room with two single beds including # Hotel Reservation Booking App

We are going to build a RESTful api for a hotel booking application.
## Assignment 1
For the first assignment you will have to create endpoints to manage hotel room and hotel guests. We can create and retrieve hotel rooms and hotel guests.
Those data will be saved into a database. 
 
### Here are the 3 endpoints for the room resource
GET:  /api/room
```json
{
  "rooms:" [
    {
      "id": "947af28f-6c93-4225-8eed-e1c72c1f722e",
      "nr": 101,
      "description": "A beautifull room with a single king size bed"
    },
    {
      "id": "8130d1bd-a01e-43dd-88b3-3d24fd472c3c",
      "nr": 203,
      "description": "A corner room with two single beds including a small kitchen"
    }
  ]
}
```
GET:  /api/room/{id}

```json
{
  "id": "8130d1bd-a01e-43dd-88b3-3d24fd472c3c",
  "nr": 203,
  "description": "A corner room with two single beds including a small kitchen"
}
```

POST: /api/room (when creating a room the backend generates a unique uuid)
```json
{
  "nr": 412,
  "description": "A penthouse type room with 2 bedrooms, 2 bathrooms, roomy living space and a kitchen"
}
```

### Here are the 2 endpoints for the guest resource

GET:  /api/guest/{id}
```json
{
  "id": "2bf657e2-00a1-4dfd-a596-efc439b2a5cd",
  "first_name": "Piet",
  "last_name": "Hein",
  "email": "piethein@test.com",
  "phone": "+3123456789",
  "details": "Alergic to nuts",
}
```
POST: /api/guest (when creating a guest the backend generates a unique uuid)
```json
{
  "first_name": "Piet",
  "last_name": "Hein",
  "email": "piethein@test.com",
  "phone": "+3123456789",
  "details": "Alergic to nuts",
}
```


#### technical requirements:
- spring boot
- MSSQL, MariaDB or PostgreDB (h2 not allowed)

  "nr": 412,
  "description": "A penthouse type room with 2 bedrooms, 2 bathrooms, roomy living space and a kitchen"
}
```

### Here are the 2 endpoints for the guest resource

GET:  /api/guest/{id}
```json
{
  "id": "2bf657e2-00a1-4dfd-a596-efc439b2a5cd",
  "first_name": "Piet",
  "last_name": "Hein",
  "email": "piethein@test.com",
  "phone": "+3123456789",
  "details": "Alergic to nuts",
}
```
POST: /api/guest (when creating a guest the backend generates a unique uuid)
```json
{
  "first_name": "Piet",
  "last_name": "Hein",
  "email": "piethein@test.com",
  "phone": "+3123456789",
  "details": "Alergic to nuts",
}
```


#### technical requirements:
- spring boot
- MSSQL, MariaDB or PostgreDB (h2 not allowed)

{
  "nr": 412,
  "description": "A penthouse type room with 2 bedrooms, 2 bathrooms, roomy living space and a kitchen"
}
```

### Here are the 2 endpoints for the guest resource

GET:  /api/guest/{id}
```json
{
  "id": "2bf657e2-00a1-4dfd-a596-efc439b2a5cd",
  "first_name": "Piet",
  "last_name": "Hein",
  "email": "piethein@test.com",
  "phone": "+3123456789",
  "details": "Alergic to nuts",
}
```
POST: /api/guest (when creating a guest the backend generates a unique uuid)
```json
{
  "first_name": "Piet",
  "last_name": "Hein",
  "email": "piethein@test.com",
  "phone": "+3123456789",
  "details": "Alergic to nuts",
}
```


#### technical requirements:
- spring boot + java
- MSSQL, MariaDB or PostgreDB (h2 not allowed)
- tests
- instructions on how to start the application

