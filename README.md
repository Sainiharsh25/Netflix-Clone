# Netflix Clone
A fully responsive Netflix clone built using the MERN stack (MongoDB, Express.js, React.js, Node.js) to replicate core features of the popular streaming platform.

## Features

- User authentication (Sign up, Log in, and Log out)
- Browse movies and TV shows
- Search for titles
- View details and trailers of movies/TV shows
- Responsive UI for mobile and desktop
- Admin dashboard for content management
- Subscription plans with payment integration (optional)

## Technologies Used

### Frontend
- React.js
- Redux Toolkit (for state management)
- Axios
- Tailwind CSS / Bootstrap (Optional: Specify CSS framework used)

### Backend
- Node.js
- Express.js

### Database
- MongoDB
- Mongoose

### Authentication
- Firebase Authentication / JSON Web Tokens (JWT)

## Installation

### Prerequisites

Make sure you have the following installed on your machine:

- Node.js (v16 or higher recommended)
- MongoDB (local instance or cloud, e.g., MongoDB Atlas)
- Git

### Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/netflix-clone.git
   cd netflix-clone
   ```

2. Install dependencies for both backend and frontend:
   ```bash
   # Install backend dependencies
   cd backend
   npm install

   # Install frontend dependencies
   cd ../frontend
   npm install
   ```

3. Set up environment variables:

   Create a `.env` file in the `backend` directory and add the following:
   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   TMDB_API_KEY=your_tmdb_api_key
   ```

4. Start the development servers:
   ```bash
   # Start the backend server
   cd backend
   npm start

   # Start the frontend server
   cd ../frontend
   npm start
   ```

5. Open your browser and navigate to:
   - Frontend: `http://localhost:3000`
   - Backend API: `http://localhost:5000`

## Project Structure

```
netflix-clone/
├── backend/
│   ├── config/       # Configuration files (e.g., database, JWT)
│   ├── controllers/  # API route controllers
│   ├── models/       # MongoDB models
│   ├── routes/       # API routes
│   ├── middleware/   # Middleware (e.g., authentication)
│   └── server.js     # Entry point for the backend
├── frontend/
│   ├── public/       # Static files
│   ├── src/
│   │   ├── components/ # React components
│   │   ├── pages/      # React pages (e.g., Home, Browse, Search)
│   │   ├── context/    # Context API for state management
│   │   └── App.js      # Main React app file
├── README.md
└── package.json      # Root package.json for the project
```

## API Endpoints

### User Routes
- `POST /api/users/register` - Register a new user
- `POST /api/users/login` - Log in a user

### Movie Routes
- `GET /api/movies` - Get all movies
- `GET /api/movies/:id` - Get movie details by ID

### Admin Routes
- `POST /api/admin/add` - Add new movies/TV shows (Admin only)
- `DELETE /api/admin/:id` - Delete movies/TV shows (Admin only)

## Future Enhancements

- Add user profiles and personalized recommendations
- Implement a payment gateway for subscription plans
- Enable content downloads for offline viewing
- Multi-language support

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature`
5. Submit a pull request

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to contact me if you have any questions or suggestions. Happy coding! 🎬

## Contact
For any questions or feedback, please feel free to contact me:

GitHub: Sainiharsh25

Email: harshsaini00025@gmail.com
