# Book Management Application

A web-based Book Management System that allows users to search for books, view their details, and manage book records effectively. This system includes features such as adding, editing, deleting, and searching for books. It uses React.js for the frontend, Node.js with Express.js for the backend, and SQLite for data storage.

## Features
- **Home Page**: Navigation bar, search section with filters (genres, authors), and search button.
- **Search Results Page**: Displays books with pagination. Options to view details, edit, or delete a book.
- **Book Details Page**: Shows detailed information about a book including title, author, genre, pages, and published date.
- **Add/Edit Book Page**: Form to add or edit book details with input validation.
- **Delete Book Confirmation**: Confirmation dialog when attempting to delete a book.

## Database Schema

### Books Table
- **BookID** (Primary Key)
- **Title**
- **AuthorID** (Foreign Key)
- **GenreID** (Foreign Key)
- **Pages**
- **PublishedDate**

### Genres Table
- **GenreID** (Primary Key)
- **Name**
- **Description**

### Authors Table
- **AuthorID** (Primary Key)
- **Name**

## Technology Stack

- **Frontend**: React.js
- **Backend**: Node.js, Express.js
- **Database**: SQLite

## Installation Instructions

### Frontend
1. Clone the frontend repository:
    ```bash
    git clone https://github.com/yourusername/book-management-frontend.git
    cd book-management-frontend
    ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Start the development server:
    ```bash
    npm start
    ```

### Backend
1. Clone the backend repository:
    ```bash
    git clone https://github.com/yourusername/book-management-backend.git
    cd book-management-backend
    ```
2. Install dependencies:
    ```bash
    npm install
    ```
3. Set up the SQLite database:
    - Make sure the SQLite database is set up correctly in the `db/` directory.
4. Start the server:
    ```bash
    node server.js
    ```

### Testing the Application

1. Open the frontend in your browser (typically at `http://localhost:3000`).
2. Use the search feature to find books, view details, and test the add/edit/delete functionality.

## API Endpoints

### **GET /books**
Fetch all books with pagination.

### **GET /books/:id**
Fetch detailed information about a specific book.

### **POST /books**
Add a new book.

### **PUT /books/:id**
Update an existing book.

### **DELETE /books/:id**
Delete a book.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
