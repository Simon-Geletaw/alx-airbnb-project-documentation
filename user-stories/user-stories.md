# 🏠 Airbnb Clone — Use Case Documentation

## 🎯 System Name
**Airbnb Clone Platform**

---

## 👥 Actors
- **Guest/User** — Can browse, book, and review properties.  
- **Host** — Can list, edit, and manage their property listings.  
- **Admin** — Manages the platform, users, properties, and bookings.

---

## 🧍‍♂️ Guest / User Use Cases

| Use Case | Description |
|-----------|--------------|
| **Register / Sign Up** | Create a new account using email and password. |
| **Log In** | Authenticate to access the platform. |
| **View Properties** | Browse or search for available properties by filters such as location, date, and price. |
| **View Property Details** | See complete property information including images, reviews, and pricing. |
| **Book Property** | Reserve a property for selected dates. |
| **Make Payment** | Complete payment for a booking via online payment gateway. |
| **View Booking History** | View all previous and current bookings. |
| **Cancel Booking** | Cancel an existing booking if allowed by the policy. |
| **Write Review** | Leave a review for a property after a stay. |
| **Log Out** | End the user session securely. |

---

## 🏡 Host Use Cases

| Use Case | Description |
|-----------|--------------|
| **Register / Log In** | Authenticate as a host on the platform. |
| **Add Property Listing** | Add a new property with details, images, and pricing. |
| **Edit Property Details** | Update existing property information. |
| **Delete Property Listing** | Remove a property from the platform. |
| **Manage Bookings** | View, accept, or reject booking requests. |
| **View Reviews** | Read feedback and ratings left by guests. |

> **Note:**  
> Both **Add Property Listing** and **Edit Property Details** *include* the sub-use case **“Enter Property Details.”**  
> This represents shared behavior (not a generalization).

---

## 🛠️ Admin Use Cases

| Use Case | Description |
|-----------|--------------|
| **Manage Users** | Add, update, or deactivate user and host accounts. |
| **Manage Properties** | Oversee property listings to ensure policy compliance. |
| **Manage Bookings** | Monitor booking activities and resolve issues. |
| **View Reports / Analytics** | Generate performance, usage, and financial reports. |

---

## 🔁 Use Case Relationships

| Relationship Type | Example |
|-------------------|----------|
| **Include** | `Book Property` → includes → `Make Payment` |
| **Include** | `Add Property Listing` → includes → `Enter Property Details` |
| **Extend** | `Log In` → extends → `Forgot Password` |
| **Extend** | `View Property Details` → extends → `Write Review` |

---

## 🗺️ System Boundary Overview

