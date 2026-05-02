# Ecommerce1.0

A full-featured e-commerce web application developed as a group project.  
The system provides an online shopping platform for customers and a management dashboard for administrators.

---

## Overview

Ecommerce1.0 is a React-based e-commerce web application that supports product browsing, shopping cart management, checkout, order tracking, user profile management, notifications, and admin management features.

The application is divided into two main roles:

- **Customer**: Browse products, manage cart, checkout, view orders, and manage profile.
- **Admin**: Manage products, orders, vouchers, reports, and store statistics.

---

## Tech Stack

- **Frontend**: React, JavaScript, TypeScript, CSS
- **Routing**: React Router DOM
- **UI & Icons**: React Icons, Lucide React
- **Charts & Reports**: Recharts
- **Notification Service**: Firebase Cloud Messaging
- **Tooling**: Node.js, npm, React Scripts

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/thongken/Ecommerce1.0.git
```

### 2. Move into the frontend folder

```bash
cd Ecommerce1.0/frontend
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm start
```

The app will run locally at:

```bash
http://localhost:3000
```

---

## Features

### Customer Features

- **Home Page**  
  Display product categories, banners, popular products, best sellers, and new arrivals.

- **Product Browsing**  
  View product lists by category and browse available products.

- **Product Details**  
  View product images, price, description, and related products.

- **Search**  
  Search for products by keyword.

- **Shopping Cart**  
  Add products to cart, update product quantity, remove items, and view cart summary.

- **Checkout**  
  Enter shipping information, preview order details, and place orders.

- **Authentication**  
  User login and protected user routes.

- **Order History**  
  View previous orders and order status.

- **Profile Management**  
  View and update user profile information.

- **Product Reviews**  
  View and submit product reviews.

- **Notifications**  
  Receive and display user notifications using Firebase Cloud Messaging.

---

### Admin Features

- **Admin Dashboard**  
  View general store statistics and dashboard information.

- **Product Management**  
  Add, edit, delete, and manage product information.

- **Order Management**  
  View customer orders and update order status.

- **Voucher Management**  
  Create, update, and delete discount vouchers.

- **Reports**  
  View reports and store performance data.

- **Admin Layout**  
  Separate admin interface with sidebar and navbar.

---

## Project Structure

```bash
Ecommerce1.0/
├── README.md
├── .gitignore
└── frontend/
    ├── public/
    │   ├── index.html
    │   ├── manifest.json
    │   ├── robots.txt
    │   └── firebase-message-sw.js
    │
    ├── src/
    │   ├── Admin/
    │   │   ├── Components/
    │   │   └── Pages/
    │   │
    │   ├── Components/
    │   │   ├── Banner/
    │   │   ├── CartItem/
    │   │   ├── Header/
    │   │   ├── Navbar/
    │   │   ├── ProductCard/
    │   │   ├── ProductDisplay/
    │   │   └── ...
    │   │
    │   ├── Context/
    │   │   ├── CartContext.jsx
    │   │   └── ShopContext.jsx
    │   │
    │   ├── Pages/
    │   │   ├── Cart.jsx
    │   │   ├── Checkout.jsx
    │   │   ├── Login.jsx
    │   │   ├── Orders.jsx
    │   │   ├── Product.jsx
    │   │   ├── Profile.jsx
    │   │   ├── SearchResults.jsx
    │   │   └── Shop.jsx
    │   │
    │   ├── api/
    │   │   ├── cartService.js
    │   │   ├── categoryService.js
    │   │   ├── dataService.js
    │   │   ├── fileService.js
    │   │   ├── geocodeService.js
    │   │   ├── locationService.js
    │   │   ├── orderService.js
    │   │   ├── paymentService.js
    │   │   ├── productService.js
    │   │   ├── reviewService.js
    │   │   ├── statisticService.js
    │   │   ├── userService.js
    │   │   └── voucherService.js
    │   │
    │   ├── assets/
    │   │   ├── logo.png
    │   │   ├── banner_all.png
    │   │   ├── hero_image.png
    │   │   └── ...
    │   │
    │   ├── data/
    │   │   ├── all_product.js
    │   │   ├── data.js
    │   │   ├── new_arrivals.js
    │   │   ├── orders.js
    │   │   └── Promo.js
    │   │
    │   ├── utils/
    │   │   ├── constantsMap.js
    │   │   ├── currencyUtils.js
    │   │   ├── dateUtils.js
    │   │   └── useDebounce.js
    │   │
    │   ├── firebase.js
    │   ├── App.js
    │   ├── App.css
    │   ├── index.js
    │   └── index.css
    │
    ├── package.json
    └── package-lock.json
```

---

## Main Pages

### Public / Customer Pages

- `/` - Home page
- `/product/:id` - Product detail page
- `/cart` - Shopping cart
- `/checkout` - Checkout page
- `/login` - Login page
- `/orders` - Order history
- `/profile` - User profile
- `/search` - Search results
- `/notifications` - User notifications

### Admin Pages

- `/admin` - Admin layout
- `/admin/dashboard` - Admin dashboard
- `/admin/products` - Manage products
- `/admin/orders` - Manage orders
- `/admin/vouchers` - Manage vouchers

---

## Screenshots

Screenshots of the application can be added here, such as:

- Home page
- Product detail page
- Shopping cart
- Checkout page
- Admin dashboard
- Product management page
- Order management page

---

## Security Note

This project may require Firebase or service account configuration for notification features.

Do not commit private key files such as:

```bash
service-account.json
```

Recommended ignored files:

```bash
.env
service-account.json
frontend/public/service-account.json
```

Sensitive files should be stored locally or configured through environment variables.

---

## Contributors

This project was developed as a group assignment.

- **Repository**: `https://github.com/thongken/Ecommerce1.0`
- **Related group repository**: `https://github.com/DangHoangThanh/EcomWebApp`

---

## About

Ecommerce1.0 is an e-commerce web application that provides online shopping features for customers and management tools for administrators.  
The project focuses on building a user-friendly shopping interface, reusable components, and a separate admin management system.
