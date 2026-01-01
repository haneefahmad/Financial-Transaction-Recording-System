# Financial Transaction Management System (Flask)

A simple Flask-based web application to manage bank transactions.
It supports Create, Read, Update, Delete (CRUD) operations, searching transactions, and calculating total balance.

---

## Features

* View all transactions
* Add new transactions
* Edit existing transactions
* Delete transactions
* Search transactions by amount range
* Display total balance dynamically
* Clean UI using Bootstrap

---

## Tech Stack

* Backend: Python, Flask
* Frontend: HTML, CSS, Bootstrap
* Templating: Jinja2

---

## Project Structure

```
project/
│
├── app.py
├── templates/
│   ├── transactions.html
│   ├── form.html
│   ├── edit.html
│   └── search.html
│
└── README.md
```

---

## How to Run the Project

### Step 1: Install Flask

```bash
pip install flask
```

### Step 2: Run the Application

```bash
python app.py
```

### Step 3: Open in Browser

```
http://127.0.0.1:5000/
```

---

## Available Routes

| Route          | Description            |
| -------------- | ---------------------- |
| `/`            | View all transactions  |
| `/add`         | Add a new transaction  |
| `/edit/<id>`   | Edit a transaction     |
| `/delete/<id>` | Delete a transaction   |
| `/search`      | Search by amount range |
| `/balance`     | View total balance     |

---

## Total Balance Feature

* Total balance is calculated by summing all transaction amounts.
* Displayed at the bottom of the transactions table.
* Also accessible via the `/balance` route.

---

## Sample Data

```python
transactions = [
    {'id': 1, 'date': '2023-06-01', 'amount': 100},
    {'id': 2, 'date': '2023-06-02', 'amount': -200},
    {'id': 3, 'date': '2023-06-03', 'amount': 300}
]
```

---

## Notes

* Data is stored in memory (no database).
* Restarting the server resets all transactions.
* This project is intended for learning Flask CRUD concepts.

---

## Author

Haneef Ahmad

---

## Future Improvements

* Database integration (SQLite or MySQL)
* Authentication and login system
* Export transactions to CSV
* Improved UI dashboards

---

