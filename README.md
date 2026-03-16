#  FastAPI Assignment 3 — Day 4 (CRUD APIs)
### Innomatics Research Labs | Data Science Internship | February 2026

---

## 📌 Overview

This repository contains FastAPI Assignment 3 (Day 4) solutions as part of the Innomatics Research Labs Data Science Internship. This assignment focuses on building a complete **CRUD API** for an E-commerce Product system using POST, PUT, DELETE, and GET endpoints.

---

## 📂 Repository Structure
```
IN226060702_FASTAPI
└── ASSIGNMENT 3
    ├── main.py
    ├── Q1_Output.png
    ├── Q1_Output2.png
    ├── Q1_Output3.png
    ├── Q2_Output.png
    ├── Q2_Output2.png
    ├── Q2_Output3.png
    ├── Q2_Output4.png
    ├── Q3_Output.png
    ├── Q3_Output2.png
    ├── Q3_Output3.png
    ├── Q4_Output1.png
    ├── Q4_Output2.png
    ├── Q4_Output3.png
    ├── Q4_Output4.png
    ├── Q4_Output5.png
    ├── Q5_Output.png
    ├── QBonus_Output1.png
    ├── QBonus_Output2.png
    └── QBonus_Output3.png
```

---

## 🧩 Tasks Completed

### ✅ Q1 — Add New Products Using POST
- Added Laptop Stand (₹1299, Electronics) with ID 5
- Added Sticky Notes (₹49, Stationery) with ID 6
- Tested duplicate product — returns 400 Bad Request

**Endpoints:** `POST /products`

---

### ✅ Q2 — Update USB Hub Using PUT
- Restocked USB Hub using `in_stock=true`
- Updated price to ₹699
- Updated both fields at once → price 649, in_stock true
- Tested non-existing ID 99 → 404 Not Found

**Endpoints:** `PUT /products/{product_id}`

---

### ✅ Q3 — Delete Pen Set
- Deleted Pen Set (ID 4) successfully
- Verified total dropped from 4 to 3
- Tested delete again → 404 Not Found

**Endpoints:** `DELETE /products/{product_id}`

---

### ✅ Q4 — Full CRUD Lifecycle for Smart Watch
- POST → Added Smart Watch (ID 7, ₹3999)
- GET → Confirmed ID
- PUT → Fixed price to ₹3499
- GET → Verified price
- DELETE → Removed Smart Watch
- GET → Confirmed Smart Watch gone

**Endpoints:** `POST` → `GET` → `PUT` → `GET` → `DELETE` → `GET`

---

### ✅ Q5 — Inventory Audit Endpoint
- Returns total products, in-stock count, out-of-stock names
- Calculates total stock value (price × 10)
- Shows most expensive product

**Endpoint:** `GET /products/audit`

---

### ⭐ Bonus — Category-Wide Discount
- Applied 10% discount to all Electronics
- Verified reduced prices
- Tested non-existing category → friendly message

**Endpoint:** `PUT /products/discount`

---

## 🚀 How to Run

**Install dependencies:**
```
pip install fastapi uvicorn
```

**Run the server:**
```
uvicorn main:app --reload
```

**Test in Swagger UI:**
```
http://127.0.0.1:8000/docs
```

---

## 🛠️ Tools & Technologies

- **Language:** Python 3
- **Framework:** FastAPI
- **Validation:** Pydantic
- **Server:** Uvicorn
- **Testing:** Swagger UI

---

## 👨‍💻 Author

**Syed Muzammil Ansar**
- 🎓 Computer Science Student
- 💼 Data Science Intern — Innomatics Research Labs
- 🔗 [LinkedIn](https://www.linkedin.com/in/syed-muzammil-ansar-0095022a7)

---

> *This project was completed as part of the Innomatics Research Labs Data Science Internship Program — February 2026.*
