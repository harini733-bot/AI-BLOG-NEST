# Phase 3 -- System Architecture

## 1. Architecture

BlogNest uses a layered backend architecture.

## 2. Request Flow

**Client → Express Server → Routing/Middleware → Controller →
Mongoose/Service → MongoDB → JSON Response**

Protected requests additionally pass through authentication and role
checks.

## 3. Components

### API Interface

Postman or Thunder Client sends HTTP requests and receives JSON
responses.

### Express Server

Handles HTTP methods, JSON payloads, routing and CORS.

### Authentication Middleware

Validates tokens and checks user roles.

### Logic Layer

Handles blog lifecycle, comments and related business rules.

### Database Layer

Uses Mongoose to work with MongoDB.

### AI Flow

Provides blog generation and summarization.

## 4. AI Request Flow

**Client → AI Route → Controller → AI Service → External Language Model
→ Generated Content/Summary → JSON Response**

## 5. Expected Workflow

A request enters an API endpoint and passes through applicable
middleware. Protected operations verify the JWT and user role. The
controller performs the required operation through the relevant model or
service. MongoDB stores or retrieves data and the API returns a JSON
response.

For AI requests, the controller delegates the task to the AI flow and
returns generated content or a summary.
