# 🚖 Taxi Booking System – Low Level Design (LLD)

## 📌 Project Overview

This project is a **Taxi Booking System** implemented in Java as part of a Low Level Design (LLD) problem.

The system simulates real-world taxi allocation based on:
- Taxi availability
- Nearest pickup location
- Fair earnings distribution
- Automatic fare calculation

It demonstrates strong understanding of **Object-Oriented Programming** and **LLD principles**.

---

## 🏗️ Problem Statement

Design a taxi booking system where:

- Multiple taxis are available.
- Taxis operate between locations (A, B, C, D...).
- Each booking includes pickup point, drop point, and pickup time.
- A taxi can be assigned only if it can reach the pickup location before the requested time.
- Among available taxis:
  1. Nearest taxi is selected.
  2. If multiple taxis are equally near, the taxi with **less total earnings** is chosen (fair distribution).

---

## 🧠 LLD Concepts Applied

✔ Class-based design  
✔ Encapsulation  
✔ Separation of concerns  
✔ Business logic abstraction  
✔ Comparator-based sorting  
✔ Real-time availability checking  

---

## 🏛️ System Design

### 🔹 Main Components

- **Booking** → Stores booking details  
- **Taxi** → Represents each taxi and its state  
- **TaxiService** → Handles booking logic and allocation  
- **Main** → Entry point of the application  

---

## 🚦 Taxi Allocation Strategy

A taxi is considered available if:

```
Taxi Free Time + Travel Time to Pickup <= Requested Pickup Time
```

Selection Priority:
1. Minimum distance to pickup point
2. Minimum total earnings (to balance revenue fairly)

---

## 💰 Fare Calculation Logic

- First 5 distance units → ₹100  
- Additional units → ₹10 per unit  

Formula:
```
Fare = 100 + (Extra Distance × 10)
```

---

## 📊 Features

- Multiple taxi management
- Automatic taxi allocation
- Fair earnings distribution
- Booking history tracking
- Total earnings display per taxi
- Console-based output display

---

## ▶️ How to Run

1. Open the project in Eclipse / IntelliJ / VS Code
2. Compile all Java files
3. Run the `Main` class
4. View booking allocation and taxi earnings in console

---

## Output

<img width="903" height="491" alt="image" src="https://github.com/user-attachments/assets/36fcde93-0698-47d6-ac55-432de4ac49f2" />


## 📈 Sample Flow

- System initialized with multiple taxis
- Customers request rides
- System checks availability
- Best suitable taxi is assigned
- Booking details are stored
- Earnings updated
- Final report displayed

---

## 🎯 Learning Outcome

Through this project, the following LLD skills are demonstrated:

- Real-world problem modeling
- Object relationship handling
- Sorting & selection logic
- Clean separation of responsibilities
- Basic simulation of a transport booking system

---

## 👩‍💻 Author

**Kowsika Muralikrishnan**

---


