# 🎬 Movie Ticket Booking System

**Internship Major Project | Backend Development**

Welcome to my first Major Project as an intern! This project is a robust, production-ready backend for a Movie Ticket Booking System built with **FastAPI**. It showcases a comprehensive implementation of modern backend development principles, ranging from data validation to complex multi-step business workflows.

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.115.0-brightgreen)](https://fastapi.tiangolo.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Uvicorn](https://img.shields.io/badge/Uvicorn-0.30.1-orange)](https://www.uvicorn.org/)

## 📋 Table of Contents

- [🎯 Project Objective](#-project-objective)
- [🚀 Key Features](#-key-features)
- [🛠 Technical Implementation](#-technical-implementation-day-1---day-6-concepts)
- [📂 Project Structure](#-project-structure)
- [⚙️ Getting Started](##-getting-started)
- [📈 Internship Progress](#-internship-progress)

---

## 🎯 Project Objective

The objective of this project was to build a fully functional FastAPI backend that integrates all concepts covered from **Day 1 to Day 6** of my internship curriculum:

- **API Development:** Implementing GET and POST endpoints.
- **Data Integrity:** Pydantic validation for incoming request bodies.
- **Logic Abstraction:** Modular helper functions for clean code.
- **Resource Management:** Full CRUD (Create, Read, Update, Delete) operations.
- **Advanced Features:** Search, Sorting, and Pagination.
- **Workflow Design:** Multi-step booking logic.

---

## 🚀 Key Features

| Feature                  | Description                                                        |
| ------------------------ | ------------------------------------------------------------------ |
| **Full CRUD Operations** | Create, read, update, delete movies & bookings with business rules |
| **Advanced Search**      | Keyword search across title, genre, language (case-insensitive)    |
| **Sorting & Pagination** | Sort by price/title/duration/seats, paginated results              |
| **Seat Hold Workflow**   | Hold → Confirm → Release multi-step booking process                |
| **Pricing Logic**        | Seat types, promo codes (SAVE10/SAVE20), dynamic calculations      |
| **Data Validation**      | Pydantic models with field constraints & custom errors             |
| **Summary Stats**        | Revenue totals, genre counts, seat availability                    |

**Core Endpoints (20+ total):**
| Category | Examples |
|----------|----------|
| Basic | `/`, `/movies`, `/movies/{id}`, `/bookings` |
| CRUD | `POST /movies`, `PUT /movies/{id}`, `DELETE /movies/{id}` |
| Advanced | `/movies/search`, `/movies/sort`, `/movies/page`, `/movies/browse` |
| Workflows | `/seat-hold`, `/seat-confirm/{id}`, `/seat-release/{id}` |

---

## 🛠 Technical Implementation (Day 1 - Day 6 Concepts)

### 1. API Architecture

```
GET APIs: Optimized endpoints for fetching movie details, theater lists, and user history.
POST APIs: Secure endpoints for user registration and booking requests using Pydantic models for request body validation.
```

### 2. Core Logic & Helpers

```
Helper Functions: Modularized utility functions for price calculations, availability checks, and format conversions.
Validation: Strict type-checking and custom error handling to ensure zero-fault data entry.
```

### 3. Data Management

```
Search: Query parameters for searching movies by title or genre.
Sorting & Pagination: Efficient data retrieval to handle large catalogs without performance degradation.
Multi-step Workflows: Logic to handle the transition from "Seat Selection" → "Validation" → "Booking Confirmation."
```

**Tech Stack:**
| Component | Technology | Purpose |
|-----------|------------|---------|
| Framework | FastAPI | REST API server |
| Validation | Pydantic | Request/Response models |
| Server | Uvicorn | ASGI production server |
| Data | In-memory lists | Development persistence |

---

## 📂 Project Structure

```
.
├── main.py              # FastAPI initialization & all endpoints (Q1-Q20)
├── requirements.txt     # Project dependencies (FastAPI, Uvicorn, Pydantic)
├── README.md            # Project documentation
└── screenshots/         # API docs & workflow screenshots
```

---

## ⚙️ Getting Started

### Prerequisites

- Python 3.8+
- Pip (Python Package Manager)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/Mangesh9i7/FASTAPI-Movie-Ticket-Booking.git
   cd FASTAPI-Movie-Ticket-Booking
   ```

2. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the server:**

   ```bash
   uvicorn main:app --reload
   ```

4. **Access Documentation:**
   Open [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs) to view interactive Swagger UI.

---

## 📈 Internship Progress

This project successfully implements the following curriculum:

| Day     | Concepts Implemented                                | Status | Key Endpoints                                   |
| ------- | --------------------------------------------------- | ------ | ----------------------------------------------- |
| **1-2** | FastAPI setup, GET/POST basics, Pydantic validation | ✅     | `/`, `/movies`, `/bookings`, `POST /bookings`   |
| **3-4** | CRUD operations, Helper function modularity         | ✅     | `POST/PUT/DELETE /movies`, helpers              |
| **5-6** | Search, Sorting, Pagination, Complex Workflows      | ✅     | `/search`, `/sort`, `/page`, seat-hold workflow |



**A fully functional, high-performance backend system for managing movie ticket bookings, built with FastAPI. This project marks my first major milestone during my internship, integrating core backend concepts from Day 1 through Day 6, including CRUD operations, multi-step workflows, and data validation.**
