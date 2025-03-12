# Backend Developer Intern Assignment

## Hosted API on Render 🚀
The backend is live and can be tested using Postman at:
**https://zylentrix-task.onrender.com**

## Setup Instructions
1. Clone the repository
```bash
  git clone your_repo_url_here
```
2. Navigate to project folder
```bash
  cd backend-intern-assignment
```
3. Install dependencies
```bash
  npm install
```
4. Create a `.env` file and add MongoDB URI:
```
MONGO_URI=your_mongodb_connection_string_here
PORT=5000
```
5. Start the server
```bash
  npm start
```

## API Endpoints
| Method | Endpoint       | Description        |
|--------|---------------|--------------------|
| POST   | `/api/users`  | Create a new user |
| GET    | `/api/users`  | Get all users     |
| GET    | `/api/users/:id` | Get user by ID |
| PUT    | `/api/users/:id` | Update user by ID |
| DELETE | `/api/users/:id` | Delete user by ID |

### Sample Request (Create User)
```json
POST /api/users
{
  "name": "John Doe",
  "email": "johndoe@example.com",
  "age": 25
}
```

### Sample Response
```json
{
  "_id": "60f5a9f9c2d1b5c89c4f3e9b",
  "name": "John Doe",
  "email": "johndoe@example.com",
  "age": 25,
  "createdAt": "2025-03-12T12:34:56.789Z",
  "updatedAt": "2025-03-12T12:34:56.789Z"
}
```

## Notes
- The API follows REST principles.
- MongoDB is used as the database.
- Basic error handling and input validation are included.
- The project is structured for scalability.
