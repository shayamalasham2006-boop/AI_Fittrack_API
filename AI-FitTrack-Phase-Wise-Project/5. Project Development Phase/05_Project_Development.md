# Phase 5 – Project Development Phase

## Technology Stack
- Node.js 20+
- Express.js
- MongoDB Atlas / MongoDB
- Mongoose
- Google Gemini SDK (`@google/genai`)
- JWT
- bcryptjs
- CORS
- Morgan
- Nodemon

## Source Structure
```text
Project Source Code/
├── src/
│   ├── app.js
│   ├── server.js
│   ├── config/db.js
│   ├── controllers/
│   │   ├── authController.js
│   │   ├── workoutController.js
│   │   └── aiController.js
│   ├── middleware/
│   │   ├── auth.js
│   │   └── errorHandler.js
│   ├── models/
│   │   ├── User.js
│   │   └── Workout.js
│   ├── routes/
│   │   ├── authRoutes.js
│   │   ├── workoutRoutes.js
│   │   ├── aiRoutes.js
│   │   └── index.js
│   └── services/
│       └── geminiService.js
├── package.json
└── FitTrack.postman_collection.json
```

## Installation
```bash
npm install
```

Create `.env` with MongoDB, JWT and Gemini credentials.

## Run
```bash
npm run dev
```
Production:
```bash
npm start
```

## Main Endpoints
- `POST /api/auth/register`
- `POST /api/auth/login`
- `GET /api/auth/profile`
- `POST /api/workouts`
- `GET /api/workouts`
- `GET /api/workouts/:id`
- `PUT /api/workouts/:id`
- `DELETE /api/workouts/:id`
- `GET /api/workouts/search?q=running`
- `POST /api/ai/workout-recommendation`
- `POST /api/ai/fitness-insights`
