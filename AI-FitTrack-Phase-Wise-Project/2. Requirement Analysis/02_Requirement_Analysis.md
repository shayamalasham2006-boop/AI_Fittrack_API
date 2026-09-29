# Phase 2 – Requirement Analysis

## Functional Requirements

| ID | Requirement | Description |
|---|---|---|
| FR-01 | Registration | Create a user account |
| FR-02 | Login | Authenticate using email and password |
| FR-03 | Profile | Retrieve authenticated user profile |
| FR-04 | Add Workout | Store workout name, category, duration, calories and date |
| FR-05 | List Workouts | Return the user's workout history |
| FR-06 | View Workout | Retrieve one workout by ID |
| FR-07 | Update Workout | Modify an owned workout |
| FR-08 | Delete Workout | Remove an owned workout |
| FR-09 | Search | Search by workout name, category or date |
| FR-10 | AI Recommendation | Generate workout recommendations from age, goal and experience |
| FR-11 | AI Insights | Generate insights from workout statistics |

## Non-Functional Requirements
- Secure authentication
- User-level data isolation
- RESTful API design
- Maintainable MVC structure
- Centralized error handling
- Database persistence
- Reliable AI service integration

## Main API Groups
- `/api/auth`
- `/api/workouts`
- `/api/ai`

## Environment Configuration
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
```
