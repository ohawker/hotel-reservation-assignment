# Hotel Reservation Booking App

We are going to build a RESTful api for a hotel booking application. This will be part one of multiple assignments and by the end of it, we should have a very basic hotel booking application. Feel free to ask the instructor for further clarification if things are unclear.

## Assignment 1
For the first assignment you will have to create endpoints to manage hotel room and hotel guests. We can create and retrieve hotel rooms and hotel guests.
The data will be saved into a sql database.

### Here are the 3 endpoints for the room resource
GET:  /api/rooms

* status: 200
* Content-Type: application/json

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
GET:  /api/rooms/{id}

* status: 200
* Content-Type: application/json

```json
{
  "id": "8130d1bd-a01e-43dd-88b3-3d24fd472c3c",
  "nr": 203,
  "description": "A corner room with two single beds including a small kitchen"
}
```

POST: /api/rooms (when creating a room the backend generates a unique uuid)

Request:
```json
{
  "nr": 412,
  "description": "A penthouse type room with 2 bedrooms, 2 bathrooms, roomy living space and a kitchen"
}
```
Response: (header and body)
* status: 201
* Content-Type: application/json
* Location: http://example.com/api/rooms/996859f1-8980-4c34-aa22-3a3fefba29eb
```json
{
  "id": "996859f1-8980-4c34-aa22-3a3fefba29eb",
  "nr": 412,
  "description": "A penthouse type room with 2 bedrooms, 2 bathrooms, roomy living space and a kitchen"
}
```

### Here are the 2 endpoints for the guest resource
Fetching a specific guest by id should produce the following

Response: (header and body)

GET:  /api/guests/{id}

* status: 200
* Content-Type: application/json
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
POST: /api/guests (when creating a guest the backend generates a unique uuid)
```json
{
  "first_name": "Piet",
  "last_name": "Hein",
  "email": "piethein@test.com",
  "phone": "+3123456789",
  "details": "Alergic to nuts",
}
```
Response: (header and body)
* status: 201
* Content-Type: application/json
Location: http://example.com/api/guests/996859f1-8980-4c34-aa22-3a3fefba29eb
```json
{
  "id": "9f34e4e9-3898-46d4-bc10-af2145d23722",
  "first_name": "Piet",
  "last_name": "Hein",
  "email": "piethein@test.com",
  "phone": "+3123456789",
  "details": "Alergic to nuts",
}
```

#### Technical requirements:
- spring boot + java
- MSSQL, MariaDB or PostgreDB (h2 not allowed)
- tests
- instructions on how to start the application

hint: for spring boot think about the controller-service-repository pattern
