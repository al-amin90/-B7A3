# 🏟️ Football Ticket Booking System

### Database Design & SQL Queries Assignment

---

## 📋 Project Overview

A simplified **Football Ticket Booking System** database built with PostgreSQL.
Covers ERD design, relational schema, and intermediate-to-advanced SQL queries.

---

## 🎯 Learning Objectives

- Design an ERD with 1-to-1, 1-to-Many, and Many-to-1 relationships
- Understand Primary Keys, Foreign Keys, and Referential Integrity
- Write SQL queries using JOIN variants, subqueries, aggregations,
  pattern matching, null handling, and pagination

## 🔗 ERD Relationships

```
USERS  ||──o{  BOOKINGS  }o──||  MATCHES
```

| Relationship         | Description                                       |
| -------------------- | ------------------------------------------------- |
| One to Many          | One User → Many Bookings                          |
| Many to One          | Many Bookings → One Match                         |
| One to One (logical) | Each Booking row = one unique User + Match + Seat |

> 📎 **ERD Link:** [View ERD on Lucidchart](https://lucid.app/lucidchart/9252bd6b-3605-4c3b-b55f-b42053d549f8/edit?viewport_loc=-905%2C-93%2C2076%2C1112%2C0_0&invitationId=inv_95cf8b61-2507-4b03-b0b6-5c65f5a98256)

---

## 🔍 SQL Queries Summary

| #   | Description                                    | Concepts Used           |
| --- | ---------------------------------------------- | ----------------------- |
| Q1  | Champions League matches with Available status | WHERE, AND              |
| Q2  | Users named Tanvir or containing Haque         | LIKE, ILIKE             |
| Q3  | Bookings with NULL payment status              | IS NULL, COALESCE       |
| Q4  | Booking details with user name and fixture     | INNER JOIN              |
| Q5  | All users including those with no bookings     | LEFT JOIN               |
| Q6  | Bookings above average total cost              | Subquery, AVG           |
| Q7  | Top 2 expensive matches skipping the highest   | ORDER BY, LIMIT, OFFSET |

---

## ⚙️ How to Run

**Requirement:** PostgreSQL installed locally or pgAdmin / any SQL client.

```bash
# Step 1 — Create the database
createdb football_booking

# Step 2 — Run schema + seed data
psql -d football_booking -f query.sql
```

# Step 3 — Run queries

---

## 📹 Viva Video

**Questions answered:**

- Question 1 — Foreign Key & Referential Integrity
- Question 2 — WHERE vs HAVING with Aggregate Functions
- Question 5 — Main Query vs Subquery And when we Subquery instead of JOIN

> 🎥 **Video Link:** [Watch Viva on Google Drive](https://drive.google.com/drive/folders/1Yu2uXnJBKIoz1OoIZQKNwrqdcT1GtaTa?usp=sharing)

---
