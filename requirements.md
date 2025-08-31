# 📄 Airbnb Clone – Backend Requirements Specification

This document outlines the **functional** and **technical** requirements for three key backend features of the Airbnb Clone project. Each section includes API endpoints, input/output specifications, validation rules, and performance expectations.

---

## 1. 🔐 User Authentication

### ✅ Functional Requirements
- Users can register as **Guest** or **Host**.
- Users must be able to **log in** and receive a **JWT token**.
- JWT is used to **authorize** protected routes.
- Users can **update their profile**.

### 📌 API Endpoints

#### POST `/api/auth/register`
**Input:**
```json
{
  "first_name": "Jane",
  "last_name": "Doe",
  "email": "jane@example.com",
  "password": "SecurePass123!",
  "role": "host"
}
