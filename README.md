# 📧 Email Campaign Builder

The **Email Campaign Builder** is a powerful, flexible tool that enables users to create, customize, and send email notifications to targeted user groups or large audiences—right from within your platform. Designed with usability and scalability in mind, it features a drag-and-drop editor, pre-built templates, scheduling, analytics, and more.

---

## 🚀 Features

- 🔧 **Drag-and-Drop Email Editor** — Build professional emails without writing code.
- 📚 **250+ Pre-built Templates** — Use industry-specific designs or customize your own.
- 🎯 **Audience Targeting** — Send emails to specific groups or mass audiences.
- ⏰ **Scheduled Sending** — Choose when to send emails or trigger based on events.
- 📊 **Analytics Dashboard** — Track delivery, opens, clicks, and campaign success.
- 🔔 **Notification System** — Automate alerts and follow-up messages.

---

## 📌 Project Purpose

This project is designed to:
- Improve internal and external communication through customizable email campaigns.
- Simplify campaign management for marketing, operations, and support teams.
- Provide a seamless, code-free experience to create professional, responsive emails.

---

## 🏗️ Architecture Overview

The Email Campaign Builder is built using a **microservices architecture**, with each domain-specific service running independently. Communication is handled via RESTful APIs, and services are designed for scalability and maintainability.

### 🔁 Development Approach

This solution follows the **Entity Framework Core Database-First approach**:

- The database schema is defined first (SQL Server).
- EF Core’s `Scaffold-DbContext` is used to generate entity models and DbContext.
- Each microservice manages its own DbContext and schema separately.
- Shared logic and infrastructure (e.g., logging, repositories) reside in a `BuildingBlocks` project.

---

## 🛠️ Tech Stack

| Layer           | Technology                          |
|----------------|--------------------------------------|
| Frontend        | Razor Pages (ASP.NET Core), Bootstrap or Tailwind CSS |
| Backend         | ASP.NET Core Web API                |
| Database        | SQL Server                          |
| ORM             | Entity Framework Core (Database-First) |
| Email Delivery  | SendGrid / Mailgun / Amazon SES     |
| Authentication  | ASP.NET Identity + JWT              |
| Scheduling      | Hangfire or Quartz.NET              |
| Logging         | Serilog or NLog                     |
| File Storage    | Azure Blob / Amazon S3 (optional)   |
