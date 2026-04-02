# Expense Tracker API (FastAPI)

## 📌 Overview

This project is a RESTful API built using FastAPI to manage and track expenses. It supports creating, updating, deleting, and retrieving expense records with JSON-based storage.

---

## 🚀 Features

* Create, update, delete, and retrieve expenses
* REST API with structured endpoints
* Data validation using Pydantic models
* JSON-based persistent storage
* Logging system for tracking API activity
* Error handling for invalid requests and duplicate entries

---

## 🧠 Tech Stack

* **Backend:** FastAPI
* **Language:** Python
* **Validation:** Pydantic
* **Server:** Uvicorn
* **Storage:** JSON file
* **Tools:** Postman

---

## ⚙️ API Endpoints

| Method | Endpoint               | Description                 |
| ------ | ---------------------- | --------------------------- |
| POST   | `/create-expense`      | Create a new expense        |
| GET    | `/list-expenses`       | Retrieve all expenses       |
| GET    | `/get-expense/{id}`    | Retrieve a specific expense |
| PUT    | `/update-expense/{id}` | Update an expense           |
| DELETE | `/delete-expense/{id}` | Delete an expense           |

---

## 📂 Project Structure

```id="exp123"
Expense-Tracker-API/
│
├── main.py                 # Entry point of FastAPI app
├── models.py               # Pydantic models
├── crud.py                 # Business logic
├── db.py                   # JSON storage handling
├── logger.py               # Logging configuration
├── expense_data.json       # Database file
│
├── routers/
│   └── expenses.py         # API routes
│
├── logs/
│   └── app.log             # Log file
│
├── Expense_Tracker_API.postman_collection.json
├── requirements.txt
└── README.md
```

---

## ▶️ Run the Application

```bash id="run123"
pip install -r requirements.txt
uvicorn main:app --reload
```

---

## 🧪 Testing

Use Postman to test the API endpoints.
A Postman collection is included in the project.

---

## 📊 Example Data

Sample expense structure:

```json id="json123"
{
  "id": "exp001",
  "title": "Groceries",
  "amount": 250.0,
  "category": "Food"
}
```

---

## ⚠️ Limitations

* Uses JSON file instead of a database
* Not optimized for concurrent access
* No authentication implemented

---

## 🔮 Future Improvements

* Add database integration (PostgreSQL / MongoDB)
* Implement authentication (JWT)
* Add user-based expense tracking
* Deploy using Docker

---

## 👨‍💻 Author

Vijay Sai Nunna

