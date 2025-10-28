# ALX Airbnb Clone - Backend Requirements

This document specifies the technical and functional requirements for key backend features of the ALX Airbnb clone project.

---

## 1. User Authentication

**Objective:** Handle user registration, login, logout, and secure access.

### API Endpoints

| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/auth/register` | POST | Register a new user |
| `/api/auth/login` | POST | Authenticate user and return a token |
| `/api/auth/logout` | POST | Logout user and invalidate token |
| `/api/auth/me` | GET | Retrieve current user profile |
