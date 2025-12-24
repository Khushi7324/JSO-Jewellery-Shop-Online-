# JSO-Jewellery-Shop-Online-
JSO (Jewellery Shop Online) is a web-based e-commerce application built using Core PHP, MySQL, HTML, CSS, and JavaScript. It provides a secure, user-friendly platform for browsing jewellery, managing carts, placing orders, tracking deliveries, and handling inventory through an admin dashboard.


# 💎 JSO - Jewellery Shop Online

![Project Status](https://img.shields.io/badge/Status-Complete-success)
![PHP](https://img.shields.io/badge/PHP-7.4%2B-blue)
![MySQL](https://img.shields.io/badge/MySQL-5.7%2B-orange)
![Frontend](https://img.shields.io/badge/Frontend-HTML5%20%7C%20CSS3%20%7C%20JS-yellow)

A premium, luxury jewellery shop management system built with **Core PHP**, **MySQL**, and **Vanilla JavaScript**. This project features a modern, glassmorphism-inspired UI with animated backgrounds, a complete e-commerce workflow, and a robust admin dashboard.

---

## 📖 Table of Contents
- [✨ Features](#-features)
- [🛠️ Tech Stack](#-tech-stack)
- [🚀 Installation & Setup](#-installation--setup)
- [📂 Project Structure](#-project-structure)
- [🗄️ Database Schema](#-database-schema)
- [📸 Screenshots](#-screenshots)
- [📞 Contact](#-contact)

---

## ✨ Features

### 🛍️ User (Customer) Module
- **Animated UI:** Beautiful CSS-only backgrounds (Gold Glitter, Diamond Shine) and glassmorphism cards.
- **Authentication:** Secure Register/Login with password hashing (`bcrypt`) and session management.
- **Product Catalog:**
  - Browse products by category (Gold, Diamond, Platinum, Silver, Gemstone).
  - Filter by price and sort by popularity/newest.
  - Live search functionality.
- **Shopping Experience:**
  - AJAX-based "Add to Cart" (no page reload).
  - Manage cart quantities and remove items.
  - Apply **Coupon Codes** for discounts.
- **Checkout & Orders:**
  - Secure checkout with address validation.
  - Pincode-based delivery feasibility check.
  - **Order Tracking:** Real-time status updates (Pending → Shipped → Delivered).
  - **Invoice Generation:** Auto-generated printable PDF invoices.
  - **Returns:** 7-day return policy management.

### 👨‍💼 Admin Module
- **Dashboard:** Analytics for Total Sales, Total Orders, and Recent Activity.
- **Product Management:** Add, Edit, Delete products with image uploads and stock tracking.
- **Order Management:** View order details, update delivery status, and process returns.
- **Inventory Control:** Monitor stock levels and manage categories.
- **User Management:** View registered users and manage roles.
- **Marketing:** Create and manage **Coupons** and **Offers**.

---

## 🛠️ Tech Stack

- **Frontend:**
  - HTML5, CSS3 (Custom Animations, Flexbox/Grid)
  - JavaScript (Vanilla JS, AJAX for async operations)
- **Backend:**
  - PHP (Core PHP, Object-Oriented style for DB)
- **Database:**
  - MySQL (Relational Data Model)
- **Server:**
  - Apache (XAMPP/WAMP)

---

## 🚀 Installation & Setup

### 1. Prerequisites
- Install **XAMPP** (or WAMP/MAMP).
- Ensure Apache and MySQL services are running.

### 2. Clone/Download
Place the project folder `JSO` inside your `htdocs` directory:
```
C:\xampp\htdocs\JSO\
```

### 3. Database Configuration
1. Open **phpMyAdmin** (`http://localhost/phpmyadmin`).
2. Create a new database named `jso_shop`.
3. Import the `database.sql` file located in the project root:
   - Click **Import** tab -> Choose File -> Select `database.sql` -> Click **Go**.
4. (Optional) If you have a separate admin setup script, run `setup_admin.php` to create the first admin user, then delete the file.

### 4. Run the Project
- **User Portal:** [http://localhost/JSO/](http://localhost/JSO/)
- **Admin Panel:** [http://localhost/JSO/admin/login.php](http://localhost/JSO/admin/login.php)

> **Default Admin Credentials:**
> - Email: `admin@example.com`
> - Password: `admin123`

---

## 📂 Project Structure

```bash
JSO/
├── admin/                  # Admin panel files
│   ├── dashboard.php       # Admin home
│   ├── products.php        # CRUD products
│   └── orders.php          # Order management
├── assets/                 # Static assets
│   ├── css/                # Stylesheets (style.css, background.css)
│   ├── js/                 # JavaScript files (main.js)
│   └── images/             # Product images & icons
├── config/
│   └── db.php              # Database connection file
├── includes/               # Reusable components
│   ├── header.php          # Navigation bar
│   ├── footer.php          # Footer section
│   └── functions.php       # Helper functions
├── tools/                  # Utility scripts
│   ├── migrate_db.php      # Database migration tool
│   └── seed_products.php   # Data seeder
├── uploads/                # User uploaded product images
├── index.php               # Homepage
├── catalog.php             # Product listing
├── product.php             # Single product detail
├── cart.php                # Shopping cart
├── checkout.php            # Order placement
└── database.sql            # Database schema import file
```

---

## 🗄️ Database Schema

The project uses a normalized relational database with **11 Tables**:

1.  **`users`**: Customer and Admin accounts.
2.  **`categories`**: Product categories (Gold, Diamond, etc.).
3.  **`products`**: Inventory items with pricing and stock.
4.  **`product_images`**: Multiple gallery images per product.
5.  **`cart`**: Temporary shopping cart data for users.
6.  **`orders`**: Order summaries (Total, Address, Status).
7.  **`order_items`**: Individual items linked to orders.
8.  **`delivery_status`**: Tracking history for orders.
9.  **`returns`**: RMA requests and return status.
10. **`coupons`**: Discount codes and validity.
11. **`reviews`**: Product ratings and comments.

---

## 📸 Screenshots

| **Homepage** | **Product Catalog** |
|:---:|:---:|
| *(Place screenshot here)* | *(Place screenshot here)* |

| **Cart & Checkout** | **Admin Dashboard** |
|:---:|:---:|
| *(Place screenshot here)* | *(Place screenshot here)* |

---

## 📞 Contact

For any queries or support, please contact the development team.

**Project Link:** [http://localhost/JSO/](http://localhost/JSO/)
