# Web Application Architecture - College Canteen Application

**USN:** NB25CSE200
**Name:** Mandal Sushant
**Subject:** Software Engineering
**Unit:** V - Software Applications and Emerging Trends

---

## Problem Statement

A college wants to build an online canteen application so that students can view the
daily menu, place food orders from their phones and avoid standing in long queues
during the lunch break. The staff need to see the incoming orders and update the
status of each one.

The task is to apply web application architecture to this system, explain each tier
with the technology used, and show how a single order flows through the application.

---

## 1. Introduction to Web Application Architecture

Most modern web applications follow a **three-tier architecture**. The work is divided
into three separate layers, and each layer has only one responsibility.

* **Presentation tier** - the user interface that runs in the browser (the client),
  written in HTML, CSS and JavaScript and built with React, Angular or Vue.js.
* **Application (logic) tier** - the server-side code that holds the business rules,
  the REST APIs and the authentication, built with Node.js/Express, Django or Spring Boot.
* **Data tier** - the database that stores the data, such as MySQL, PostgreSQL or MongoDB.

A request from the browser always travels over the internet to the application server.
The server applies the business rules, queries the database and sends back HTML or JSON.
The browser never talks to the database directly.

---

## 2. Architecture Diagram

```
                  HTTP Request                               SQL Query
                    ------->                                  ------->
 +------------+                  +----------------------+                  +------------+
 |  Browser   |                  |  Application Server  |                  |  Database  |
 |  (Client)  |                  |        / API         |                  |  (MySQL)   |
 +------------+                  +----------------------+                  +------------+
                    <-------                                  <-------
                Response (JSON)                              Result Set

 Presentation Tier               Application / Logic Tier                    Data Tier
```

> **Memory tip - the canteen app in 3 boxes:** Browser (menu, cart) -> Server (order,
> payment) -> Database (students, orders).

---

## 3. Applying the Architecture to the Canteen Application

| Tier | Technology | What it contains in this system |
|---|---|---|
| Tier 1 - Presentation (client) | React / Angular / Vue, HTML, CSS, JS | Daily menu page, item search, cart and checkout page, student login and sign-up, order status screen, responsive layout for mobile |
| Tier 2 - Application / logic | Node.js with Express, Django or Spring Boot (REST APIs) | Student service for authentication, menu service, cart and order service that calculates the bill, payment service that calls the payment gateway, notification service for the counter |
| Tier 3 - Data | MySQL / PostgreSQL / MongoDB | Students table, menu items and daily availability, orders and order items, payments, token numbers and order status |

---

## 4. Working: How One Order Flows

1. The student opens the canteen website and the browser sends an HTTP request to
   load the menu for the day.
2. The application server calls the menu service, which queries the database for the
   items available that day and returns the list as JSON.
3. The student adds items to the cart and clicks **Place Order**. The server checks
   that the items are still in stock, calculates the total with tax, and calls the
   payment gateway.
4. On a successful payment, the order is saved in the Orders table, a token number is
   generated and the canteen counter is notified.
5. The order status screen asks the server for updates, and the server reads the
   current status from the database and shows it to the student as Preparing, Ready or
   Collected.

---

## 5. Advantages of This Architecture

**Separation of concerns.** The UI, the business logic and the data are independent, so
the menu page can be redesigned without touching the order logic or the database.

**Scalability.** More application servers can be added during the lunch rush, when
hundreds of students order at the same time, and removed afterwards. This is called
scaling out.

**Security.** The database is never exposed directly to the browser. Every request
passes through the application tier, which checks the student's login first.

**Reach.** A responsive design or a PWA lets the same site work on a phone, so students
do not need to install a separate app.

---

## 6. Conclusion

With a three-tier architecture the canteen application has a clean browser interface, a
scalable business-logic layer and a secure database. Each tier can be developed, tested
and maintained on its own, and the system can grow as more students start using it.

---

### References

1. Unit 5 Notes
2. Sommerville, *Software Engineering*, 9th Edition - p.494, Figure 18.10
