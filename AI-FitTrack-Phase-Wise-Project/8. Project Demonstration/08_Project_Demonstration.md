# Phase 8 – Project Demonstration

## Demo Flow

### 1. Install and Start
```bash
npm install
npm run dev
```

### 2. Register
`POST /api/auth/register`

### 3. Login
`POST /api/auth/login`
Save the JWT token.

### 4. View Profile
`GET /api/auth/profile` with Bearer token.

### 5. Add Workout
`POST /api/workouts`
```json
{
  "workoutName": "Evening Jog",
  "category": "Running",
  "duration": 30,
  "caloriesBurned": 350
}
```

### 6. View / Update / Delete
Demonstrate:
- `GET /api/workouts`
- `GET /api/workouts/:id`
- `PUT /api/workouts/:id`
- `DELETE /api/workouts/:id`

### 7. Search
`GET /api/workouts/search?q=running`

### 8. AI Recommendation
`POST /api/ai/workout-recommendation`
```json
{
  "age": 22,
  "fitnessGoal": "Weight Loss",
  "experience": "Beginner"
}
```

### 9. AI Fitness Insights
`POST /api/ai/fitness-insights`
```json
{
  "totalWorkouts": 18,
  "averageDuration": 45,
  "totalCaloriesBurned": 6300
}
```

### 10. Presentation Points
- Problem statement
- Proposed solution
- Architecture
- MongoDB schema
- JWT security
- Workout CRUD/search
- Gemini AI integration
- Testing
- Future enhancements
