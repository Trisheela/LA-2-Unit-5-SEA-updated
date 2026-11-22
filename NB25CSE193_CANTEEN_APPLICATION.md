# Mobile and Web Applications Engineering – Online Canteen Food-Ordering System

*Name:* M Sohail Nawaz  
*USN:* NB25CSE193  
*Section:* C  
*Subject:* Software Engineering  
*Case Study:* Online Canteen Food-Ordering System

## 1. Introduction

Mobile and web applications are software applications designed to provide services through smartphones, tablets and computers.

A mobile application is installed on a mobile device, whereas a web application runs through a web browser. A Progressive Web Application (PWA) combines useful features of both mobile and web applications.

For a college canteen, an online food-ordering system can help students browse food items, place orders, make payments and receive notifications when their food is ready.

## 2. Problem Analysis

In a traditional college canteen, students usually stand in queues to check menus, place food orders and make payments. During busy hours, this process can result in overcrowding, delays and confusion.

The college needs an online food-ordering application that allows students to order food conveniently without waiting in long queues.

The proposed system should provide an easy-to-use interface for students and an order management facility for canteen staff.

## 3. Comparison of Mobile, Web and Progressive Web Applications

### Mobile Application

- Installed directly on smartphones.
- Can use device features such as cameras and notifications.
- Requires separate development or adaptation for different platforms.

### Web Application

- Accessed through a web browser.
- Does not require installation.
- Can be used on different devices with internet access.
- May have limited access to certain device features.

### Progressive Web Application (PWA)

- Works through a web browser.
- Can be added to the home screen.
- Supports responsive design and eligible push notifications.
- Can provide selected offline features.

### Comparison Table

| Feature | Mobile App | Web App | PWA |
|---|---|---|---|
| Installation | Required | Not required | Optional |
| Accessibility | Mobile devices | Browser devices | Browser devices |
| Updates | App updates | Server updates | Server updates |
| Notifications | Supported | Browser-dependent | Supported on eligible platforms |
| Offline support | Possible | Limited | Possible with caching |

## 4. Selection of Suitable Application

A Progressive Web Application (PWA) is a suitable choice for the college canteen food-ordering system.

Reasons for selecting PWA:

1. Students can access it through a browser without downloading a separate application.
2. It works across different devices and operating systems.
3. It can be added to the home screen for easy access.
4. It supports push notifications on compatible browsers and devices.
5. It reduces development and maintenance effort compared with maintaining separate mobile applications.

Therefore, a PWA provides a convenient and cost-effective solution for the college canteen.

## 5. Major Functionalities

### 1. Student Registration and Login

Students can create accounts and securely log in to access the food-ordering system.

### 2. Food Menu Display

The application displays available food items with names, prices, descriptions and availability.

### 3. Online Ordering and Payment

Students can select food items, add them to the cart, confirm their orders and make online payments through an integrated payment gateway.

### 4. Order Tracking and Notifications

Students can view their order status and receive notifications when the order is accepted, prepared and ready for collection.

## 6. Application Workflow Diagram

mermaid
flowchart TD
A[Student Opens PWA] --> B[Login or Register]
B --> C[Browse Food Menu]
C --> D[Select Food Items]
D --> E[Add Items to Cart]
E --> F[Confirm Order]
F --> G[Online Payment]
G --> H[Order Sent to Canteen]
H --> I[Food Preparation]
I --> J[Order Ready Notification]
J --> K[Student Collects Food]


## 7. Development Challenges

1. *Payment Security:* Protecting student payment details and ensuring secure online transactions.
2. *Internet Connectivity:* Students need a reliable internet connection for placing and tracking orders.
3. *Order Management:* Handling multiple orders during peak hours without delays or incorrect deliveries.

## 8. Benefits

- Reduces waiting time and overcrowding in the canteen.
- Makes food ordering easier and faster.
- Provides real-time order status updates.
- Improves order management for canteen staff.
- Offers convenient access through different devices.

## 9. Conclusion

A Progressive Web Application is a suitable solution for developing an online college canteen food-ordering system. It provides easy accessibility, convenient ordering, online payments and order notifications.

By implementing this system, the college canteen can improve its service quality, reduce waiting time and provide a better experience for students and staff.
