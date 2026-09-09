# pantry-app

A simple Python backend to track ingredients at home and practice building REST APIs. 

## Why I built this
I wanted a hands-on project to practice data modeling and basic CRUD operations. To keep myself focused, I **time-boxed the initial build to one week** so I would focus on finishing a working application rather than getting lost in feature creep.

## Tech Stack
* **Language:** Python
* **Framework:** FastAPI
* **Database:** SQLite
* **Tools:** Git, Virtual Environments (venv)

## What it does (Features)
* Lets you Add, View, Update, and Delete (CRUD) pantry items.
* Stores basic item data: name, quantity, and unit (e.g., "1 Litre of Milk").
* Uses a simple, flat API structure so it's easy to expand later.

**Example API Endpoints**

The backend exposes a small REST-style API for managing pantry items.



```http

### Health check

Returns a simple response to verify that the API is running.
GET /

Response:

{ "message": "Hello Pantry!" }

List pantry items

GET /pantry

Add a pantry item

POST /pantry
Content-Type: application/json

{
  "name": "Milk",
  "amount": 1,
  "unit": "l"
}

Update a pantry item (replace fields)

PUT /pantry/{item_id}
Content-Type: application/json

{
  "name": "Milk",
  "amount": 2,
  "unit": "l"
}

Delete a pantry item

DELETE /pantry/{item_id}
```


**Project Status**

This project is under active development.
Current focus is on solidifying core CRUD functionality before expanding into recipes and shopping list features.

**Project Scope**

This project was time-boxed to one week in order to practice scoping, prioritization, and finishing a usable application within a limited timeframe.

**Future Improvements**

Partial updates (PATCH) and more granular field updates

Recipe-to-ingredient linking

Shopping list generation

Basic frontend interface

Exploring price comparison using external data sources (where available)


**Why This Project Exists**

I came up with the idea on a personal need. I want to be the kind of engineer who builds their own tools when a need arises.
This project was created as a hands-on exercise to practice:

Finishing and iterating on an idea

Backend application structure

Database modeling

Writing maintainable code
