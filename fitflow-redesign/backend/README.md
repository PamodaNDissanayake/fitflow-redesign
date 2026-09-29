# FitFlow Backend

## Purpose

Provide secure APIs for FitFlow clients and coordinate
database operations and AI requests.

## Proposed Technologies

- Node.js
- Express
- TypeScript
- Cloud Firestore
- Firebase Authentication
- Redis when shared caching or rate limiting is required

## Main Responsibilities

- Verify Firebase ID tokens.
- Validate incoming requests.
- Check record ownership and circle membership.
- Store approved workout plans and workout records.
- Store confirmed meal records.
- Manage private circles and community posts.
- Send authorized requests to the AI service.
- Prevent duplicate records during offline synchronization.

## Proposed API Endpoints

| Method | Endpoint | Purpose |
|---|---|---|
| POST | /v1/plans/generate | Request a workout suggestion |
| POST | /v1/plans | Save an approved workout plan |
| POST | /v1/workout-events | Record workout activity |
| POST | /v1/meals | Save a confirmed meal |
| POST | /v1/circles | Create a private circle |
| POST | /v1/circles/{circleId}/posts | Share a post |
| GET | /v1/progress | Retrieve progress summaries |

These endpoints are proposed contracts, not implemented routes.

## Security

- Require authentication for protected endpoints.
- Check authorization for each resource.
- Keep service credentials outside the repository.
- Avoid recording health information in application logs.
- Validate uploaded image type and size.
- Use unique event IDs to prevent duplicate submissions.

Server access to Firestore must enforce authorization explicitly;
privileged server SDK operations do not rely on client Security Rules.

## Status

Planning stage. Backend implementation has not started.