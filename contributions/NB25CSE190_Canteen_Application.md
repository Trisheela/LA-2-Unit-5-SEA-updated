Question 2: Mobile and Web Applications Engineering
A college plans to develop an online canteen food-ordering system that allows students to browse menus, place orders, make payments, and receive notifications when their orders are ready.
Analyze whether a mobile application, web application, or Progressive Web Application (PWA) would be suitable for this system. Justify your choice and explain the major functionalities and development challenges.
Expected contribution:
●	Introduction to mobile and web applications
●	Comparison of mobile, web, and PWA approaches
●	Selection of a suitable application type with justification
●	Four major functionalities
●	Three development challenges
●	Simple application workflow diagram
# Question 2: Mobile and Web Applications Engineering

## 1. Introduction to Mobile and Web Applications

Mobile and web applications are software applications developed to provide services to users through digital devices.

- **Mobile Application:** An application installed on smartphones or tablets. It can access device features and provide notifications.
- **Web Application:** An application accessed through a web browser without installing it on the device.
- **Progressive Web Application (PWA):** A web application that combines the features of websites and mobile applications. It can be installed on the home screen, supports notifications on compatible devices, and provides limited offline functionality.

For the college canteen, these applications can help students browse food menus, place orders, make payments, and receive notifications when their food is ready.

## 2. Comparison of Mobile, Web, and PWA Approaches

| Features | Mobile Application | Web Application | PWA |
|---|---|---|---|
| Installation | Required | Not required | Optional |
| Accessibility | Through mobile devices | Through web browsers | Browser and home screen |
| Platform Support | Android/iOS | Multiple platforms | Multiple platforms |
| Notifications | Supported | Limited browser support | Supported on compatible devices |
| Offline Access | Possible | Usually limited | Supports cached content |
| Development Cost | High | Moderate | Moderate |
| Maintenance | App updates required | Centralized updates | Centralized updates |

## 3. Selection of Suitable Application Type

For the college canteen food-ordering system, a **Progressive Web Application (PWA)** is the most suitable choice.

### Justification:

1. **Easy Accessibility:** Students can access the application through a web browser without downloading it from an app store.
2. **Cost-Effective:** A single application can work across different devices and operating systems.
3. **Push Notifications:** Students can receive notifications when their orders are ready, provided their browser and device support them.
4. **Home-Screen Installation:** Students can add the application to their mobile home screens for quick access.
5. **Offline Support:** Previously loaded menus and basic information can be accessed through cached content, even when internet connectivity is unavailable.

Therefore, a PWA provides the advantages of both mobile and web applications while reducing development and maintenance costs.

## 4. Four Major Functionalities

### a) Menu Browsing
- Displays available food items with images, prices, and descriptions.
- Allows students to view different food categories.
- Shows the availability of food items.

### b) Online Food Ordering
- Allows students to select food items.
- Provides an option to add items to the shopping cart.
- Allows students to confirm and place orders.

### c) Online Payment
- Supports digital payment methods such as UPI, debit cards, and net banking.
- Provides payment confirmation after successful transactions.
- Maintains payment and transaction records.

### d) Order Tracking and Notifications
- Displays the current status of the order.
- Updates students when their orders are accepted, being prepared, or ready for collection.
- Sends notifications when the food is ready, reducing waiting time.

## 5. Three Development Challenges

### a) Payment Security
Protecting students' payment information and ensuring secure transactions can be challenging.

**Solution:** Use secure payment gateways, HTTPS encryption, and proper user authentication.

### b) Real-Time Order Management
Managing multiple orders simultaneously and updating order status without delays can be difficult.

**Solution:** Use a real-time database and efficient order management techniques.

### c) Cross-Device Compatibility
The application must work properly on different smartphones, screen sizes, browsers, and operating systems.

**Solution:** Use responsive web design and test the PWA on different devices and browsers.

## 6. Simple Application Workflow Diagram

```text
          STUDENT OPENS PWA
                  |
                  v
             STUDENT LOGIN
                  |
                  v
            BROWSE FOOD MENU
                  |
                  v
           SELECT FOOD ITEMS
                  |
                  v
              ADD TO CART
                  |
                  v
          CONFIRM FOOD ORDER
                  |
                  v
          MAKE ONLINE PAYMENT
                  |
                  v
          ORDER CONFIRMATION
                  |
                  v
          CANTEEN RECEIVES ORDER
                  |
                  v
            FOOD PREPARATION
                  |
                  v
           ORDER STATUS UPDATED
                  |
                  v
          NOTIFICATION SENT
                  |
                  v
          STUDENT COLLECTS FOOD
```



