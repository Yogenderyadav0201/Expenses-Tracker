# Expenses-Tracker
Expenses Tracker


expense-tracker/
├── backend/
│   ├── models/
│   │   └── Expense.js
│   ├── routes/
│   │   └── expenses.js
│   ├── server.js
│   └── .env
├── react-expenses/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── ExpenseForm.js
│   │   │   ├── ExpenseList.js
│   │   ├── App.jsx
│   │   ├── index.css
│   │   └── App.css
│   └── package.json
├── README.md
└── package.json

Step-1 Download the backend.zip and react-expenses.zip and unzip these two folder
Step-2 How run/installation the backend

  npm init -y
  npm install express cors dotenv
  
  use this command for run
  npm server.js

  Goto this url for check all data display in JSON format.
  http://localhost:8989/expenses


Step-3 How to run the react-expenses 

  npm install
  npm run dev

  Goto this url
  http://localhost:5173/

  



Step-4 used the postgresql database:-

CREATE TABLE expenses (
    id SERIAL PRIMARY KEY,
    amount NUMERIC(10, 2) NOT NULL,
    category VARCHAR(255) NOT NULL,
    description TEXT,
    date DATE NOT NULL
);


INSERT INTO expenses (amount, category, description, date)
VALUES
    (100.50, 'Food', 'Lunch at a restaurant', '2025-01-01'),
    (200.00, 'Transportation', 'Taxi fare', '2025-01-02'),
    (50.00, 'Entertainment', 'Movie ticket', '2025-01-03'),
    (300.75, 'Shopping', 'Clothing purchase', '2025-01-04'),
    (150.00, 'Bills', 'Electricity bill', '2025-01-05'),
    (90.25, 'Groceries', 'Weekly groceries', '2025-01-06');

