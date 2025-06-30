
# 🌐 Virtual Community Support Platform

A comprehensive full-stack web application that bridges the gap between volunteers and social organizations. Designed to promote social impact, this platform allows users to discover missions (social service opportunities), contribute their time and skills, and build stronger communities.

---

## 📌 Table of Contents

- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Project Modules](#-project-modules)
- [Architecture Overview](#-architecture-overview)
- [Database Schema](#-database-schema)
- [Installation Guide](#-installation-guide)
- [API Overview](#-api-overview)
- [Future Scope](#-future-scope)
- [License](#-license)
- [Contact](#-contact)

---

## 🚀 Features

### User Features
- 🔐 Secure Registration & Login
- 🎯 Explore & Apply for Social Missions
- 🌍 Country & City-based Filtering
- ⭐ Mission Rating & Feedback
- 📅 View and Manage Mission History

### Admin Features
- 👤 User Management (Volunteers & CMS Users)
- 📌 Create, Edit & Delete Missions
- 🧠 Manage Skills, Themes, Countries & Cities
- 📊 View Mission Applications & Volunteer Statistics

### Additional
- 📄 Dynamic CMS Pages
- 📨 Contact Us Form
- 🔎 Search & Pagination Support

---

## 🛠️ Tech Stack

### Backend
- **Language:** C#
- **Framework:** ASP.NET Core MVC (Web API)
- **ORM:** Entity Framework Core
- **Database:** SQL Server
- **IDE:** Visual Studio 2022

### Frontend
- **Framework:** Angular
- **Styling:** Bootstrap 5 / TailwindCSS
- **Tools:** HTML, CSS, JavaScript, jQuery
- **IDE:** Visual Studio Code

---

## 🧱 Project Modules

```plaintext
Mission/                - ASP.NET Core Web API (Controllers, Startup configs)
Mission.Entities/       - Entity Framework Models and DbContext
Mission.Repositories/   - Data Access Layer (Repositories & Interfaces)
Mission.Services/       - Business Logic Layer (Service Classes)
```

Each module plays a crucial role in separating concerns and maintaining a clean architecture:
- **Entities:** Contains database models and relationship mapping.
- **Repositories:** Responsible for querying data and interacting with the database.
- **Services:** Contains core business rules and validation logic.
- **Mission:** Main API project with controllers, middlewares, startup files, and routing.

---

## 🏗️ Architecture Overview

- **Layered Architecture:** Clean separation of concerns between DAL, BLL, and Web
- **Repository Pattern:** Abstracts database operations
- **Dependency Injection:** For services and repositories
- **REST API Design:** Follows standard conventions for endpoints

---

## 🗃️ Database Schema (Sample Entities)

- `Users` - Stores volunteer & admin credentials
- `Missions` - Mission info, duration, availability
- `MissionApplications` - Tracks applications per user
- `Skills` - Specific skill requirements for missions
- `Countries` & `Cities` - Location management
- `CMSPages` - Static content managed by admin

---

## 🧪 Installation Guide

### 🔧 Prerequisites

- Visual Studio 2022 or later
- VS Code
- Angular
- .NET 8 SDK
- SQL Server (PostgreSQL)
- Git (to clone repo)

### 🛠️ Steps

#### 🔷 For Backend:
1. Clone the repository:
   ```bash
   git clone https://github.com/Punit231/Virtual-Community-Support.git
   ```
2. Open `Mission.sln` in Visual Studio.
3. Configure your connection string in:
   ```
   Mission/appsettings.json
   ```
4. Apply EF Core Migrations:
   ```bash
   Update-Database
   ```
5. Run the application:
   ```bash
   F5 or Ctrl+F5
   ```

#### 🔷 For Frontend:
1. Navigate to the frontend directory (e.g., `cd Frontend`).
2. Install dependencies:
   ```bash
   npm install
   ```
3. Run the development server:
   ```bash
   npm run dev
   ```
4. The app should now be running at `http://localhost:3000`

---

## 🌐 API Overview

Sample APIs:

| Method | Endpoint 	   | Description            |
|--------|-----------------|------------------------|
| GET    | `/api/missions` | Get all missions       |
| POST   | `/api/apply`    | Apply for a mission    |
| GET    | `/api/skills`   | Fetch available skills |
| POST   | `/api/login`    | User authentication    |

> Full Swagger documentation available at `/swagger` once project is running.

---

## 🔮 Future Scope

- ✅ Role-based authorization using JWT
- ✅ Email notification system for mission status
- 🌐 Multi-language support
- 📱 Mobile App version (React Native / Flutter)
- ☁️ Deploy on Azure / AWS with CI/CD

---

## 📄 License

This project is licensed under the **MIT License**.  
Feel free to use, share, and improve this project.

---

## 📬 Contact

- 📧 Email: punitparmar231@gmail.com
- 🔗 LinkedIn: www.linkedin.com/in/punitparmar231

> _“Be the change you wish to see in the world.” — Mahatma Gandhi_
