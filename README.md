# Book Store Project

A full-stack web application for managing a book store, built with the MERN stack (MongoDB, Express.js, React, Node.js). This project allows users to perform CRUD (Create, Read, Update, Delete) operations on books.

## Features

- **View Books**: Display all books in a table or card format
- **Add New Books**: Create new book entries with title, author, and publish year
- **Edit Books**: Update existing book information
- **Delete Books**: Remove books from the collection
- **Responsive Design**: Works on desktop and mobile devices
- **Real-time Notifications**: User feedback for all operations using toast notifications

## Tech Stack

### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database (using MongoDB Atlas)
- **Mongoose** - MongoDB object modeling
- **CORS** - Cross-origin resource sharing

### Frontend
- **React** - JavaScript library for building user interfaces
- **Vite** - Build tool and development server
- **React Router** - Declarative routing for React
- **Axios** - HTTP client for API requests
- **Notistack** - Notification library for React
- **React Icons** - Icon library
- **ESLint** - Linting utility

## Project Structure

```
book_store_project/
├── backend/
│   ├── config.js          # Database and server configuration
│   ├── index.js           # Main server file
│   ├── models/
│   │   └── bookModel.js   # Book data model
│   ├── routes/
│   │   └── booksRoute.js  # API routes for books
│   └── package.json
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/    # Reusable UI components
│   │   │   ├── BackButton.jsx
│   │   │   ├── Spinner.jsx
│   │   │   └── home/
│   │   │       ├── BookModal.jsx
│   │   │       ├── BooksCard.jsx
│   │   │       ├── BookSingleCard.jsx
│   │   │       └── BooksTable.jsx
│   │   ├── pages/         # Page components
│   │   │   ├── CreateBooks.jsx
│   │   │   ├── DeleteBook.jsx
│   │   │   ├── EditBook.jsx
│   │   │   ├── Home.jsx
│   │   │   └── ShowBook.jsx
│   │   ├── App.jsx        # Main app component
│   │   ├── main.jsx       # App entry point
│   │   └── assets/        # Static assets
│   ├── package.json
│   ├── vite.config.js
│   └── eslint.config.js
└── README.md
```

## Prerequisites

Before running this application, make sure you have the following installed:

- **Node.js** (version 14 or higher) - [Download here](https://nodejs.org/)
- **npm** or **yarn** - Package manager (comes with Node.js)
- **MongoDB Atlas** account - For cloud database (or local MongoDB instance)

## Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd book_store_project
   ```

2. **Install backend dependencies:**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies:**
   ```bash
   cd ../frontend
   npm install
   ```

## Configuration

### Backend Configuration

The backend configuration is in `backend/config.js`. The current setup uses MongoDB Atlas. If you want to use a local MongoDB instance, update the `mongoDBURL` in `config.js`:

```javascript
export const mongoDBURL = "mongodb://localhost:27017/books-collection";
```

### Environment Variables (Optional)

For production deployment, consider using environment variables for sensitive data like database URLs.

## Running the Application

### Development Mode

1. **Start the backend server:**
   ```bash
   cd backend
   npm run dev
   ```
   The backend will run on `http://localhost:5555`

2. **Start the frontend development server:**
   ```bash
   cd frontend
   npm run dev
   ```
   The frontend will run on `http://localhost:5173` (default Vite port)

3. **Open your browser and navigate to:**
   ```
   http://localhost:5173
   ```

### Production Build

1. **Build the frontend:**
   ```bash
   cd frontend
   npm run build
   ```

2. **Start the backend in production:**
   ```bash
   cd backend
   npm start
   ```

## API Endpoints

The backend provides the following REST API endpoints:

- `GET /` - Welcome message
- `GET /books` - Get all books
- `GET /books/:id` - Get a specific book by ID
- `POST /books` - Create a new book
- `PUT /books/:id` - Update a book by ID
- `DELETE /books/:id` - Delete a book by ID

## Database Schema

### Book Model
```javascript
{
  title: String (required),
  author: String (required),
  publishYear: Number (required)
}
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the ISC License - see the package.json files for details.

## Acknowledgments

- This project is based on a MERN stack tutorial
- Built with modern JavaScript and React best practices
- Uses MongoDB Atlas for cloud database hosting