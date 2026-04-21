## Book Store Project
A full-stack web application for managing a book store, built with the MERN stack (MongoDB, Express.js, React, Node.js). This project allows users to perform CRUD (Create, Read, Update, Delete) operations on books.

---

### Features
- **View Books**: Display all books in a table or card format
- **Add New Books**: Create new book entries with title, author, and publish year
- **Edit Books**: Update existing book information
- **Delete Books**: Remove books from the collection
- **Responsive Design**: Works on desktop and mobile devices
- **Real-time Notifications**: User feedback for all operations using toast notifications

---

### Tech Stack
#### Backend
- **Node.js** - JavaScript runtime
- **Express.js** - Web application framework
- **MongoDB** - NoSQL database (using MongoDB Atlas)
- **Mongoose** - MongoDB object modeling
- **CORS** - Cross-origin resource sharing

#### Frontend
- **React** - JavaScript library for building user interfaces
- **Vite** - Build tool and development server
- **React Router** - Declarative routing for React
- **Axios** - HTTP client for API requests
- **Notistack** - Notification library for React
- **React Icons** - Icon library
- **ESLint** - Linting utility

---

### Project Structure
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
---

### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Keerthana-webdev/book-store-project.git
   cd book_store_project
   ```

2. **Install backend dependencies:**
   ```bash
   cd backend
   npm install
   ```

3. **Install frontend dependencies:**
   ```bash
   cd frontend
   npm install
   ```
---

### Running the Application
1️⃣ **Start the backend server:**
   ```bash
   cd backend
   npm run dev
   ```
   The backend will run on `http://localhost:5555`

2️⃣ **Start the frontend development server:**
   ```bash
   cd frontend
   npm run dev
   ```
   The frontend will run on `http://localhost:5173` (default Vite port)

3️⃣ **Open your browser and navigate to:**
   ```
   http://localhost:5173
   ```
---

### API Endpoints
The backend provides the following REST API endpoints:

- `GET /` - Welcome message
- `GET /books` - Get all books
- `GET /books/:id` - Get a specific book by ID
- `POST /books` - Create a new book
- `PUT /books/:id` - Update a book by ID
- `DELETE /books/:id` - Delete a book by ID

---

### Author

#### Keerthana S
