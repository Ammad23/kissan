# 🌾 KISSAN – E-Commerce Platform (Pakistan)

## Overview

KISSAN is a multi-vendor e-commerce platform designed for Pakistan, supporting local payment methods, bilingual experience (English & Urdu), and role-based access for customers, vendors, and administrators.

This document outlines the technical foundation, architecture decisions, and recommended development roadmap.

---

## 🔒 Core Decisions (Frozen)

To ensure stability and avoid constant changes during development, the following decisions are finalized:

* **Project Name:** KISSAN
* **Country:** Pakistan
* **Languages:** English, Urdu
* **Authentication:** NextAuth
* **Database:** PostgreSQL
* **Media Storage:** Cloudinary

### 💳 Payment Methods

* Cash on Delivery (COD)
* JazzCash
* Easypaisa
* Local Card Gateway

### 👥 User Roles

* Customer
* Vendor
* Admin

---

## 🏗️ Technical Foundation

The initial development phase focuses on setting up the core architecture:

### Project Setup

* Create Next.js application
* Enable TypeScript
* Configure Tailwind CSS
* Integrate Shadcn UI

### Backend Setup

* Configure Prisma ORM
* Connect PostgreSQL database
* Set up NextAuth authentication

### Application Structure

Organize the app using route groups:

* `storefront/` – Customer-facing UI
* `vendor/` – Vendor dashboard
* `admin/` – Admin panel

---

## 🗄️ Database Schema Design

Before building UI components, define the database schema to support business logic.

### Core Models

* Users
* Vendors
* Customers
* Categories
* Products
* Inventory
* Prices
* Carts
* Orders
* Order Items
* Payments
* Commissions
* Payouts

This schema acts as the backbone of the entire application.

---

## 🔐 Authentication & Authorization

After schema setup, implement:

* Customer authentication
* Vendor authentication
* Admin authentication
* Role-based route protection

This ensures secure and structured access control early in development.

---

## 🚀 MVP Development Roadmap

Build features in the following order:

1. Vendor / Product / Category Management
2. Inventory & Pricing System
3. Storefront Product Browsing
4. Cart & Checkout Flow
5. Payment Integration
6. Order Management System
7. Vendor Dashboard
8. Admin Dashboard
9. Urdu Localization & UX Polish

---

## ⚡ Immediate Next Steps

Focus on one of the following deliverables:

### Option 1: Project Skeleton

* Folder structure
* Configurations
* Package setup
* Base layouts
* Authentication wiring

### Option 2: Prisma Schema

* Define all models
* Set enums
* Establish relationships

---

## ✅ Recommended Approach

The most effective next step:

> **Build the Prisma schema and app folder structure together**

### Benefits:

* Strong backend foundation
* Clear development direction
* Reduced rework later

---

## 🧭 Best Practical Sequence

1. Create app structure
2. Define Prisma schema
3. Configure NextAuth
4. Implement role-based layouts
5. Build vendor product management
6. Develop storefront (browsing → checkout)

---

## 📌 Recommendation

The next ideal deliverable:

* Full KISSAN project folder structure
* Initial Prisma schema (with relationships and enums)

---

## 📖 Notes

* Focus on scalability from the start (multi-vendor complexity)
* Keep localization (Urdu) in mind during UI development
* Payment integrations should be modular for flexibility

---

**KISSAN is not just an app — it’s a scalable commerce ecosystem tailored for Pakistan.**
