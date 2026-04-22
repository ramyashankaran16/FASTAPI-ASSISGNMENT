# FASTAPI-ASSISGNMENT


# 🏥 Doctor & Patient Management API

A simple REST API built using FastAPI to manage doctors and patients.
This project demonstrates basic CRUD-like operations using in-memory storage.

---

## Features

* Create and retrieve doctors
* Create and retrieve patients
* Fetch doctor by ID
* Uses UUID for unique identification
* Built with FastAPI for high performance APIs

---

## Tech Stack

* Python
* FastAPI
* Pydantic

---

## Project Structure

```
project/
│── main.py          # FastAPI application
│── Module.py        # Pydantic models (Doctor, Patient)
│── database.py      # In-memory lists (doctors, patients)
```

---

## How to Run

1. Navigate to your project folder:

```
cd path/to/your/project
```

2. Run the server:

```
uvicorn main:app --reload
```

3. Open your browser:

* API: http://127.0.0.1:8000
* Docs (Swagger UI): http://127.0.0.1:8000/docs

---

## API Endpoints

### 🩺 Doctor APIs

#### Create Doctor

```
POST /doctors
```

Request Body:

```json
{
  "name": "Dr. John",
  "specialization": "Cardiology",
  "experience": 10
}
```

#### Get All Doctors

```
GET /doctors
```

#### Get Doctor by ID

```
GET /doctors/{doctor_id}
```

---

### Patient APIs

#### Create Patient

```
POST /patients
```

Request Body:

```json
{
  "name": "Ramya",
  "age": 25,
  "phone": "9876543210"
}
```

#### Get All Patients

```
GET /patients
```

---

## Notes

* Data is stored in memory (not persistent)
* Restarting the server will clear all data
* This is a beginner-friendly demo project


---

## Author

Ramya

---
