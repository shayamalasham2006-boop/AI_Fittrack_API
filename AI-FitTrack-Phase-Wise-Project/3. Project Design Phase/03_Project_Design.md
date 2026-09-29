# Phase 3 – Project Design Phase

## Architecture
```text
Client / Postman
       |
       v
   Express API
       |
 +-----+------------------+
 |                        |
Auth Middleware       Route Layer
 |                        |
JWT verification      Controllers
                          |
            +-------------+-------------+
            |             |             |
         MongoDB       Workout       Gemini AI
        /Mongoose       Logic         Service
            |             |             |
            +-------------+-------------+
                          |
                     JSON Response
```

## MVC Structure
- `models/` – User and Workout schemas
- `controllers/` – authentication, workout and AI business logic
- `routes/` – API endpoints
- `middleware/` – JWT and error handling
- `services/` – Gemini integration
- `config/` – MongoDB configuration

## Database Design
### User
`name`, `email`, `password`, timestamps

### Workout
`user`, `workoutName`, `category`, `duration`, `caloriesBurned`, `workoutDate`, timestamps

## Security Design
- bcryptjs password hashing
- JWT bearer authentication
- Workout ownership checks
- Protected workout and AI endpoints

## AI Design
Gemini service exposes reusable functions for workout recommendations and fitness insights, while controllers validate request data before calling the service.
