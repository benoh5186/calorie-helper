# calorie-helper
## Description
Personal app that generates daily calories and macros based on user's fitness goal. 
## Tech stack
Frontend: React Native, TypeScript
Backend: Python, FastAPI 
Database: PostgreSQL
Infrastructure: AWS

## Features
Services offered by this app + flow of it

### Calories 
- Displays user's daily calories + macros
- Displays feedback if user is above or under their calories and/or macros
- Calories resets at the end of the day(12 am)
- Updates weekly based on user's weekly weigh in
- Offers user to change daily calories if their fitness goal is not met by deadline

### Steps
- Frontend makes api call to device's OS and displays total steps for every 1000 steps or whenever user hits refresh on steps page or dashboard
- Make API call to backend to POST total steps in a day at the end of the day
- Displays total calories burned
- Adds to daily calories every 2-3k steps

### Food Log
- use some api to get nutritional fact of the food user is trying to log(needs some research)
- adds to daily calories + macros
- When no internet, displays feedback

### Dashboard
- Displays calories, steps, and food log
- based on user's performance(steps, calories, macros), get json data from backend for feedback(whenever user accesses the dashboard)

### Goals
For when user first signs up or when user decides to change their goal or when user has met their fitness goal
- Asks for user's stats: Age, gender, weight, height
- Ask for user's fitness goal: cut or bulk
- saves user's info
- makes api call to get daily calories + steps 
