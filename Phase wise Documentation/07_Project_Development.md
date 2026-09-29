# Phase 5 -- Project Development

## 1. Development Stack

-   Node.js
-   Express.js
-   MongoDB
-   Mongoose
-   JWT
-   bcrypt.js
-   Google Gemini AI

## 2. Project Setup

1.  Create the project folder.
2.  Create and open the Server folder in VS Code.
3.  Run `npm init -y`.
4.  Create `server.js`.
5.  Create `models`, `controllers` and `routes`.
6.  Install Mongoose using `npm install mongoose`.
7.  Configure MongoDB connection and schemas/models.

## 3. Backend Layers

-   Routes
-   Middleware
-   Controllers
-   Models
-   AI services
-   MongoDB database

## 4. Authentication and Security

-   JWT for stateless authentication.
-   bcrypt.js for password hashing.
-   Role-based route protection.
-   Request validation.
-   Input sanitization.
-   Rate limiting.
-   Structured logging.

## 5. Blog Features

The backend supports blog content management, categories/tags, comments
and the documented lifecycle: Draft → Pending Approval → Scheduled →
Published.

## 6. AI Features

### Generate Blog

Endpoint documented in the report: `/api/ai/generate-blog`

The service takes a high-level topic or theme and produces structured
blog content using an external language model.

### Summarize

Endpoint documented in the report: `/api/ai/summarize`

The service processes longer article content and produces a concise
summary.

## 7. Source Code Upload

Place the actual working backend source code in this phase folder. Do
not upload secrets such as database passwords, JWT secrets or Gemini API
keys.
