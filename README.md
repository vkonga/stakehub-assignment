# Order Management Dashboard

This project is a simple order management dashboard built using React for the frontend and Express with SQLite for the backend. It allows users to view pending and completed orders, and manage orders through an API.


## Features

- Display pending and completed orders in separate tables.
- Real-time loading spinner while fetching data.
- Simple and clean UI built with React.
- RESTful API with Express for managing orders.
- SQLite database for storing orders.

## Installation

### Backend

1. **Clone the repository**:
   
    git clone https://github.com/your-username/stakehub-backend.git
    cd backend
    

2. **Install dependencies**:
   
    npm install express sqlite3 sqlite nodemon cors

3. **Start the backend server**:
   node app.js or nodemon app.js
   The server will start on `http://localhost:8000`.

### Frontend

1. **Navigate to the frontend directory**:
    
    cd frontend
    

2. **Install dependencies**:
    npm install react-spinners 
3. **Start the frontend server**:
    
    npm start
   The frontend will start on `http://localhost:3000`.

## Running the Project

1. **Start the backend server**:
    
    cd backend
    node app.js

2. **Start the frontend server**:
   
    cd frontend
    npm start

   The frontend will be accessible at `http://localhost:3000` and the backend API at `http://localhost:8000`.

## Endpoints

### Backend API

- `GET /pending-orders/`: Fetch all pending orders.
- `GET /completed-orders/`: Fetch all completed orders.
- `POST /orders/`: Create a new order (either buyer or seller).

### Example Order Object

json
{
  "buyer_qty": 10,
  "buyer_price": 100,
  "seller_price": 95,
  "seller_qty": 8
}
