# Online Canteen Food-Ordering System

**Name:** KRITI ANEJA  
**USN:** NB25CSE178  
**Semester:** 3  
**Section:** C  
**Faculty:** Ms. Trisheela S  

## 1. Introduction to Mobile and Web Applications

A mobile application is usually installed on a smartphone or tablet. It can use device features such as notifications. A web application runs in a browser and can be opened using a URL.

A Progressive Web Application (PWA) is a web application that provides an app-like experience. It can be opened in a browser, added to a device's home screen, and designed to support features such as notifications and limited offline access.

## 2. Problem Analysis

The college wants an online canteen system where students can view the menu, place food orders, make payments, and get notified when their orders are ready.

Ordering only at the counter can lead to long queues, especially during lunch breaks. Students may not know which food items are available, and canteen staff may find it difficult to manage many orders at once.

The proposed system should make ordering easier for students and help canteen staff manage orders properly.

## 3. Comparison of Mobile, Web and PWA

| Criteria | Mobile Application | Web Application | PWA |
|---|---|---|---|
| Access | Usually installed from an app store. | Opened through a browser. | Opened in a browser and can be added to the home screen. |
| Installation | Usually requires installation. | No installation required. | No traditional app-store installation required. |
| Device support | May need separate versions for different platforms. | Works on devices with a compatible browser. | Uses a responsive design for different screen sizes. |
| Updates | Usually updated through app stores. | Updated on the server. | Updates can be delivered through the web. |
| Offline support | Can be designed for offline use. | Usually needs internet access. | Can provide limited offline access if designed for it. |

## 4. Selection of a Suitable Application

A Progressive Web Application (PWA) is suitable for the college canteen food-ordering system. Students can open it using a link on their phones, tablets, or computers without downloading an application from an app store. They can also add it to their home screen for easier access.

The college can maintain one application for different devices. Menu items and prices can be updated centrally, so students can see the latest menu when connected to the internet. Some information can be cached for limited offline access, but placing orders and confirming payments will require an internet connection.

Therefore, a PWA is a suitable choice because it is easy to access and provides an app-like experience across devices.

## 5. Major Functionalities

### 5.1 Student Registration and Login

Students can create an account or log in using their college details. This helps the system identify each student and keep their order history.

### 5.2 Menu Browsing and Food Selection

The application displays food names, descriptions, prices, and availability. Students can select food items, choose quantities, and add them to their cart. Unavailable items should be clearly shown.

### 5.3 Order Placement and Online Payment

Students can review their cart, confirm the order, and select a payment method. The system should show an order confirmation after the payment is verified. Payments should be handled through a secure payment gateway.

### 5.4 Order Tracking and Notifications

Students can check whether their order is Received, Preparing, or Ready for Pickup. A notification can be sent when the food is ready, and the current status should also be visible in the application.

## 6. Development Challenges

### 6.1 Network and Connectivity Issues

Students may have slow or unstable internet connections on campus. The application should show clear messages when the connection fails and should prevent the same order from being submitted more than once.

### 6.2 Payment Security and Privacy

The system must protect student information and payment transactions. It should use HTTPS, secure login, and a trusted payment gateway. Sensitive payment details should not be stored unnecessarily.

### 6.3 Managing Orders During Peak Hours

Many students may place orders during lunch breaks. The system should handle multiple orders at the same time, update food availability, and help staff process orders in sequence.

## 7. Application Workflow Diagram

```text
[ Student opens the PWA ]
          |
          v
[ Login / Register ]
          |
          v
[ Browse menu and select food ]
          |
          v
[ Add items to cart ]
          |
          v
[ Confirm order and make payment ]
          |
          v
[ System verifies order and payment ]
          |
          v
[ Canteen receives and prepares order ]
          |
          v
[ Student gets a Ready for Pickup notification ]
          |
          v
[ Student collects the order ]
```

## 8. Conclusion

A Progressive Web Application can be an effective solution for the college canteen food-ordering system. It allows students to view menus, place orders, make payments, and track their orders through a browser. It is accessible on different devices and can provide an app-like experience. Connectivity, payment security, and managing orders during busy hours must be handled properly to make the system useful for students and canteen staff.
