# Phase 6 – Project Testing

## Test Cases
| ID | Test | Expected Result |
|---|---|---|
| TC-01 | Register valid user | 201 Created |
| TC-02 | Duplicate email | Validation error |
| TC-03 | Valid login | Token returned |
| TC-04 | Invalid login | 401 response |
| TC-05 | Profile without token | 401 response |
| TC-06 | Add valid workout | Workout created |
| TC-07 | List workouts | Current user's workouts returned |
| TC-08 | Get invalid workout | Not found |
| TC-09 | Access another user's workout | Not allowed |
| TC-10 | Update owned workout | Updated workout returned |
| TC-11 | Delete owned workout | Success message |
| TC-12 | Search by category | Matching workouts returned |
| TC-13 | Search by date | Matching date records returned |
| TC-14 | AI recommendation with missing input | 400 response |
| TC-15 | AI recommendation valid input | Gemini recommendation returned |
| TC-16 | AI insights valid input | Gemini insight returned |

## Security Tests
- Missing bearer token
- Invalid token
- Cross-user workout access
- Password handling

## AI Tests
Test beginner/weight-loss recommendation, different experience levels, and fitness statistics with valid and invalid inputs.

## Test Tool
The supplied `FitTrack.postman_collection.json` can be imported into Postman for API testing.
