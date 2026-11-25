# Question 2: Mobile and Web Applications Engineering

## Case Study: Online Canteen Food-Ordering System

**Name:** Madhusudhan M R 
**USN:** NB25CSE191  
**Subject:** Software Engineering and Applications (Unit V)  
**Assigned Case Study:** Question 2 – Mobile and Web Applications Engineering  

### 1. Introduction

Mobile and web applications help users access services through
smartphones, tablets, and computers. A web application runs through a
web browser, while a mobile application is installed on a mobile device.
A Progressive Web Application (PWA) combines features of websites and
mobile applications. It can be accessed through a browser and can also
be installed on a device.

For the college canteen, an online food-ordering system can allow
students to view the menu, order food, make payments, and receive
notifications when their orders are ready.

### 2. Problem Analysis

The college wants to reduce long queues and make the food-ordering
process easier. Students may have limited break time and may need to
wait in line to check the menu, place an order, and collect food. The
canteen also needs an organized way to receive and manage orders.

A digital ordering system can solve these problems by allowing students
to place orders before reaching the counter.

### 3. Proposed Solution

A **Progressive Web Application (PWA)** is a suitable choice for the
college canteen system.

A PWA can be opened using a browser on a mobile phone or computer.
Students can also add it to their device's home screen. It does not
require a separate installation through an app store, making it
convenient for students.

#### Comparison of Mobile, Web and PWA Applications

  -----------------------------------------------------------------------
  Feature           Mobile            Web Application   Progressive Web
                    Application                         Application (PWA)
  ----------------- ----------------- ----------------- -----------------
  Access            Installed on a    Opened through a  Opened through a
                    mobile device     web browser       browser and can
                                                        be installed

  Installation      Usually requires  No installation   Can be added to
                    an app store      required          the home screen

  Updates           Updated through   Updates are       Updates are
                    the app store or  available on the  generally
                    device settings   website           delivered through
                                                        the web

  Device support    Depends on the    Works on          Works on
                    supported mobile  supported         supported
                    platform          browsers          browsers and
                                                        devices

  Internet access   Some features may Usually needs     Some features can
                    work offline      internet access   work offline
  -----------------------------------------------------------------------

#### Justification for Selecting PWA

1.  Students can access the system using a browser without downloading a
    large application.
2.  It can be used on different devices, including smartphones, tablets,
    and computers.
3.  It can be added to the home screen for quick access.
4.  It is easier to maintain one application for multiple device types.
5.  It can support notifications on compatible browsers and devices.

### 4. Major Functionalities

1.  **Menu Display:** Students can view available food items, prices,
    and descriptions.
2.  **Online Ordering:** Students can select food items, add them to a
    cart, and place orders.
3.  **Online Payment:** The system can provide a secure payment option
    for completing orders.
4.  **Order Notifications:** Students can receive updates about order
    confirmation and when food is ready.
5.  **Order Management:** Canteen staff can view incoming orders and
    update their status.

### 5. Development Challenges

1.  **Payment Security:** The system must protect students' payment
    information and use a secure payment service.
2.  **Internet Connectivity:** Students may face difficulties placing
    orders when their internet connection is poor.
3.  **Order Management:** The system must handle many orders during busy
    break times and avoid duplicate or incorrect orders.

### 6. Application Workflow Diagram

``` mermaid
flowchart TD
    A[Student opens the PWA] --> B[Views the canteen menu]
    B --> C[Selects food items]
    C --> D[Adds items to cart]
    D --> E[Places the order]
    E --> F[Makes payment]
    F --> G[Order is sent to canteen]
    G --> H[Canteen prepares the order]
    H --> I[Student receives notification]
    I --> J[Student collects the food]
```

### 7. Conclusion

A Progressive Web Application is a suitable solution for the college
canteen food-ordering system. It provides easy access, supports
different devices, and reduces the need for students to wait in long
queues. Although payment security, internet connectivity, and order
management are important challenges, proper development and testing can
make the system reliable and convenient.
