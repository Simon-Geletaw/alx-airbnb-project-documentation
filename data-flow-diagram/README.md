# Airbnb Clone Project – System Overview

## Overview
This project is a clone of Airbnb, designed to simulate an online property rental platform.  
The system allows guests to search, book, and review properties, while hosts can manage their listings and receive payments.

---

## System Components

### External Entities
- **Guest**: Can search for properties, register, log in, book, and review properties.  
- **Host**: Can register, log in, add, edit, or delete properties, and receive payments.  
- **Payment Gateway**: Handles payment transactions.  

---

### Processes
1. **Registration**: Accepts registration info (email, password, profile data) and stores it in the User table.  
2. **Log in**: Accepts credentials, verifies them against the User table, returns success or failure.  
3. **Search**: Allows guests to search properties based on filters (location, price, amenities).  
4. **Add Property**: Hosts can add new property listings with details stored in the Property table.  
5. **Edit/Delete Property**: Hosts can modify or remove their listings.  
6. **Booking Creation**: Guests can book properties; booking data is stored in the Booking table.  
7. **Booking Status**: Tracks pending, confirmed, canceled, or completed bookings.  
8. **Review and Rating**: Guests can submit reviews stored in the Review table.  
9. **Payment**: Handles transactions between guests and hosts, stored in Payment records.

---

### Data Stores (Tables)
- **User Table**: Stores guest and host information.  
- **Property Table**: Stores property listings and details.  
- **Booking Table**: Stores booking information and status.  
- **Review Table**: Stores guest reviews and ratings.  
- **Payment Table**: Stores payment transactions.

---

### Data Flow Summary
- Guests and Hosts interact with the system through registration, login, booking, property management, and review processes.  
- Processes communicate with corresponding data stores to read and write data.  
- Payment information flows to the Payment process and external payment gateways.  

---

### DFD Diagram
The DFD represents the flow of information between external entities, processes, and data stores:  

![Airbnb Clone DFD](./airbnb_dfd.png)

---

### Notes
- All external entities interact with processes, **never directly with data stores**.  
- Processes are labeled in **verb-noun format**.  
- Data flows indicate **specific information** being transmitted (e.g., login credentials, booking info).  
- For readability, consider splitting this DFD into **Level 1 diagrams** per main module (User, Booking, Payment, Property).  

---

## Author
**Your Name**  
Airbnb Clone Project – Data Flow Diagram Documentation
