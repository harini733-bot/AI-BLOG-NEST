# Phase 6 -- API Testing

## Testing Tool

Postman or Thunder Client.

## Test Case 1 -- User Registration

**Purpose:** Verify new-user registration.

**Action:** Send valid registration data.

**Expected:** A new user record is created and the API returns its
implemented success response.

## Test Case 2 -- User Login

**Purpose:** Verify authentication.

**Action:** Send valid login credentials.

**Expected:** The implemented login response provides authenticated
access/token information.

## Test Case 3 -- Create Blog

**Purpose:** Verify authorized blog creation.

**Action:** Send an authenticated request with valid blog data.

**Expected:** A blog record is created.

## Test Case 4 -- Fetch Blogs

**Purpose:** Verify retrieval of blog records.

**Action:** Send the implemented blog retrieval request.

**Expected:** The API returns available blog records according to its
access rules.

## Test Case 5 -- AI Blog Generation

**Endpoint:** `/api/ai/generate-blog`

**Purpose:** Verify AI generation.

**Expected:** Generated structured blog content is returned for a valid
request.

## Test Case 6 -- Blog Summarization

**Endpoint:** `/api/ai/summarize`

**Purpose:** Verify summarization.

**Expected:** A concise summary is returned for valid article content.

## Security Testing

-   JWT validation.
-   Role-based route protection.
-   Request validation.
-   Input sanitization.
-   Rate limiting.

## Evidence

Add actual Thunder Client/Postman screenshots for each successful test
and relevant error/authorization tests.
