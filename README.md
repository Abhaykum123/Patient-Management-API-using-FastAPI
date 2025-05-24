# 🏥 Patient Management API using FastAPI
This project is a simple and functional RESTful API built with FastAPI for managing patient records. It supports creating, retrieving, and sorting patient data while also calculating BMI and providing a health verdict based on BMI.

### 🚀 Features
<ul>
<li>
  📌 Create and retrieve patient records
</li>
<li>
🧮 Automatically compute BMI and provide a verdict (Underweight, Normal, Overweight, Obese)
</li>
<li>
📊 Sort patients by height, weight, or BMI
</li>
<li>
✅ Built-in validation using Pydantic
</li>
<li>
💾 Persistent storage using a JSON file
</li>
<li>
🛡️ Robust error handling and clear API responses
</li>
</ul>

---

## 📁 Project Structure
```
├── FastAPI.py          # Main FastAPI application
├── patients.json       # JSON file used as a mock database
└── README.md           # Project documentation
```
---
## 📦 Requirements
<li>
  Python 3.8+
</li>
<li>
  FastAPI
</li>
<li>
  Uvicorn
</li>
<li>
Pydantic
</li>
<br>
Install dependencies using:

```
pip install fastapi uvicorn
```

## ▶️ Getting Started
### Run the application locally:
```
uvicorn FastAPI:app --reload
```
### Access the interactive API docs at:
<li>
Swagger UI: http://127.0.0.1:8000/docs
</li>
<li>
ReDoc: http://127.0.0.1:8000/redoc
</li>

---
## 🔧 API Endpoints

| Method | Endpoint        | Description                    |
| ------ | --------------- | ------------------------------ |
| GET    | `/`             | Welcome message                |
| GET    | `/about`        | About the API                  |
| GET    | `/view`         | View all patients              |
| GET    | `/patient/{id}` | View patient by ID             |
| GET    | `/sort`         | Sort by height, weight, or BMI |
| POST   | `/create`       | Add a new patient              |

---
## 📌 Example Request
POST /create
```
{
  "id": "P007",
  "name": "John Doe",
  "city": "Delhi",
  "age": 30,
  "gender": "male",
  "height": 1.75,
  "weight": 70
}
```
The response includes the calculated bmi and verdict.

---
## All Feature in FastAPI
![Screenshot 2025-05-25 005520](https://github.com/user-attachments/assets/84db17e9-cc02-4d1f-a4e9-cd48bc9ab548)

---
## 📖 Future Improvements
<li>
Integration with a real database (e.g., SQLite, PostgreSQL)
</li>
<li>
Add PUT and DELETE endpoints for full CRUD functionality
</li>
<li>
Build a frontend UI to interact with the API
</li>
<li>
Add authentication and user management
</li>

---

## 💡 Author
### Abhay Kumar

 Let's connect on [LinkedIn](https://www.linkedin.com/in/abhay-kumar-aa1a9129a?lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base_contact_details%3BiN9yMzITTT%2Bw7fOOwaUDpQ%3D%3D)<br>
Check out more of my work on [GitHub](https://github.com/Abhaykum123)


