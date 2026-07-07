# GreenBowl

An ASP.NET Core MVC prototype of a **Quality Assurance and Inventory Management System** created for the Canadian eco-food company **GreenBowl**.

The project digitises paper-based manufacturing, inventory and QA workflows while preserving the structure of the original production documentation used by the company.

---

# Features

## Inventory Management

- Product Inventory
- Ingredient Inventory
- Automatic inventory calculations
- Product sales
- Invoice generation

## Production Management

- Product Lot creation
- Ingredient Lot generation
- Batching Control
- Packaging Control
- Processing Control
- Equipment Check
- X-Ray Monitoring
- Bulging Test

## Quality Assurance

- QA validation
- Automatic QA status calculation
- Batch-based production records
- 15-minute production checks

## Security

- ASP.NET Identity
- Authentication
- Role-based authorization
- Admin/User separation

---

# Technology Stack

### Backend

- ASP.NET Core MVC
- Entity Framework Core
- Oracle Database
- ASP.NET Identity

### Frontend

- Razor Views
- Bootstrap
- Partial Views
- View Models

### Other

- C#
- LINQ
- REST principles
- MVC Architecture

---

# Project Structure

```
GreenBowl
│
├── Controllers
├── Models
├── ViewModels
├── Views
├── Services
├── Data
├── Areas
└── wwwroot
```

---

# Main Functionality

### Product Inventory

Manage finished products and automatically calculate:

- Batch Weight
- Produced Pouches
- Rejected Products
- Product Available For Sale
- Actual Inventory
- Productivity
- QA Status

---

### Ingredient Inventory

Manage ingredient deliveries.

Features include:

- Automatic Ingredient Lot generation
- Supplier information
- Truck information
- Quality inspection

---

### Production Forms

Each production lot contains multiple QA forms including:

- Batching
- Packaging
- Processing
- Equipment
- X-Ray
- Bulging

Most forms are split into four production batches:

- Batch A
- Batch B
- Batch C
- Batch D

---

### Automatic Calculations

The system automatically updates inventory values using production data.

Examples include:

- Batch Weight
- Total Production
- Rejections
- Inventory
- Productivity
- Product Available For Sale

---

### Automatic Lot Generation

Ingredient lots are generated automatically.

Example:

```
RI000001
RI000002
RI000003
```

The prefix is derived from the ingredient name while the numeric suffix is generated sequentially.

---

### Automatic 15-Minute Checks

Packaging and processing forms automatically generate inspection records every 15 minutes between the selected start and finish time.

---

# Architecture

The project follows the ASP.NET MVC architecture.

```
Browser
     │
     ▼
Razor Views
     │
Controllers
     │
Services
     │
Entity Framework Core
     │
Oracle Database
```

The application also makes extensive use of:

- View Models
- Partial Razor Views
- ViewData
- Dependency Injection
- Shared Services

---

# User Roles

## Administrator

- Full access
- Delete inventory
- Manage production data

## Standard User

- Create and edit records
- Cannot delete inventory

---

# Demo Credentials

Administrator

```
Email:
admin@admin

Password:
Admin123!
```

Regular users can also register through the application.

---

# Interesting Technical Features

- Automatic Ingredient Lot generation
- Automatic Product Lot generation
- Dynamic inventory calculations
- Automatic QA completion detection
- Automatic 15-minute inspection generation
- Batch-based production architecture
- Shared View Models across complex forms

---

# Future Improvements

- Complete remaining production forms
- Improve inventory update synchronization
- Extend role-based permissions
- Production deployment
- Additional reporting and analytics

---

# Author

**Ihor Zlenko**

BSc Computing

London Metropolitan University
