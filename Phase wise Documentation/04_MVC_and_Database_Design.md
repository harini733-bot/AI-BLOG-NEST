# Phase 3 -- MVC and Database Design

## 1. MVC Structure

### Model

Defines Mongoose schemas, validation, defaults and database structure.

### Controller

Processes requests, applies logic, communicates with models and returns
JSON responses.

### View / Routing Layer

BlogNest is a headless API. Routes act as the interface between HTTP
requests and controller functions.

## 2. Database

MongoDB is the primary database and Mongoose provides the ODM layer.

## 3. User Entity

-   `_id` -- ObjectId primary key
-   `name` -- required string
-   `email` -- required and unique
-   `password` -- required hashed password
-   `role` -- role value, with reader as the documented default

## 4. Post Entity

-   `_id` -- ObjectId primary key
-   `userID` -- reference to User
-   `name` -- blog title
-   `photo` -- image/path information
-   `message` -- blog content
-   `likes` -- number, default 0
-   `timestamps` -- enabled

## 5. Comment Entity

Comment is one of the documented core entities. The available report
does not specify its complete field-level schema, so
implementation-specific fields should be taken from the actual source
code.

## 6. Relationships

-   One User can have many Posts.
-   One User can create many Comments.
-   One Post can have many Comments.

## 7. Blog Lifecycle

1.  Draft
2.  Pending Approval
3.  Scheduled
4.  Published
