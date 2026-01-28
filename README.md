# pantry-app
A small personal project for managing pantry items and simple recipes, built to practice backend development and basic CRUD operations.


**Overview**

The Pantry App helps keep track of ingredients stored at home and supports adding, editing, and removing items as they are used or restocked.
The goal of the project is to practice building a simple, practical application with a clear data model and clean structure.


**Features**

Create, read, update, and delete pantry items

Store item name, quantity, and unit

Basic recipe support (work in progress)

Simple API structure designed for future expansion

CRUD operations for pantry items via a FastAPI REST-style API

**Tech Stack**

Backend: Python, FastAPI

Database: SQL (SQLite)

API: REST-style endpoints

Tools: Git, virtual environment


**Example API Endpoints**

The backend exposes a small REST-style API for managing pantry items.

### Health check

```http
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

This project was created as a hands-on exercise to practice:

Finishing and iterating on a real, usable idea

Backend application structure

Database modeling

Writing maintainable code
