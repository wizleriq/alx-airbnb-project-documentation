# Airbnb Clone — Backend Requirements

This document outlines the technical and functional requirements for key backend features of the Airbnb Clone project.

---

## 1. User Authentication

### Functional Requirements
- Users must be able to register with **email, username, and password**.
- Users must be able to log in securely using JWT tokens.
- Passwords must be hashed before storage.
- Logged-in users can update their profile.

### API Endpoints
- `POST /api/auth/register` → Register a new user  
- `POST /api/auth/login` → Authenticate and return JWT  
- `GET /api/auth/profile` → Retrieve user profile (Auth required)  
- `PUT /api/auth/profile` → Update user profile (Auth required)  

### Input / Output Specifications
- **Input (Register):**
  ```json
  {
    "username": "wisdom",
    "email": "wisdom@example.com",
    "password": "securePass123"
  }
