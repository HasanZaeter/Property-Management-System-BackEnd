<p align="center">
  <a href="http://nestjs.com/" target="blank">
    <img src="https://nestjs.com/img/logo-small.svg" width="120" alt="Nest Logo" />
  </a>
</p>

<p align="center">
  <b>Property Management System - Backend</b><br/>
  A scalable, modular, and secure backend system for managing real estate properties, built with <a href="http://nestjs.com/" target="_blank">NestJS</a> following Clean Architecture principles.
</p>

<p align="center">
<a href="https://www.npmjs.com/~nestjscore" target="_blank">
  <img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" />
</a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank">
  <img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" />
</a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank">
  <img src="https://img.shields.io/npm/dm/@nestjs/common.svg" alt="NPM Downloads" />
</a>
<a href="https://circleci.com/gh/nestjs/nest" target="_blank">
  <img src="https://img.shields.io/circleci/build/github/nestjs/nest/master" alt="CircleCI" />
</a>
<a href="https://discord.gg/G7Qnnhy" target="_blank">
  <img src="https://img.shields.io/badge/discord-online-brightgreen.svg" alt="Discord"/>
</a>
</p>

---

## 📌 About the Project  

The **Property Management System (PMS)** is a backend service for managing **properties, offices, tenants, invoices, roles/permissions, and notifications** in a unified platform.  

It is mainly built for:  
- 🏢 **Real estate agencies** that manage multiple properties.  
- 👨‍💼 **Office managers** to control listings, invoices, and clients.  
- 👥 **Tenants and property owners** to track payments, documents, and contracts.  

The system follows **Domain-Driven Design (DDD)** and **Clean Architecture** to maintain clean and scalable code.  

---

## 🚀 Features  

- 🏘 **Property & Office Management**: Create, update, and manage properties and offices.  
- 📑 **Invoice & Payments**: Attach invoice documents, track payments, and update statuses.  
- 🔑 **Authentication & Authorization**: Role-based access control (RBAC) with JWT.  
- 📬 **Notifications System**: Real-time notifications with read/unread status.  
- 📊 **Reports & Statistics**: Track top-rated properties and office performance.  
- 📷 **File Uploads**: Upload and manage property images/documents.  
- 🔍 **Search & Filtering**: Advanced property search by location, type, and status.  
- 📜 **API Documentation**: Fully documented APIs using **Swagger**.  

---

## 🛠 Tech Stack  

- **Framework**: [NestJS](https://nestjs.com/)  
- **Database**: PostgreSQL (via [TypeORM](https://typeorm.io/))  
- **Authentication**: JWT (JSON Web Token)  
- **File Storage**: Local storage (configurable to S3/Cloud)  
- **Validation**: Class-validator & Pipes  
- **API Docs**: Swagger  
- **Testing**: Jest (unit & e2e)  

---

## 🏗 Project Architecture  

The project is structured using **Clean Architecture** & **DDD (Domain-Driven Design)**:  

- **Domain Layer** → Core business logic & entities  
- **Application Layer** → Use cases & services  
- **Infrastructure Layer** → Database, repositories, external APIs  
- **Presentation Layer** → REST API (controllers & interceptors)  

This ensures **loose coupling**, **testability**, and **scalability**.  

---

## ⚙ Installation & Setup  

```bash
# Clone the repository
git clone https://github.com/OnlyAbdullh/Property-Management-System-BackEnd.git

# Navigate into the project
cd Property-Management-System-BackEnd

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env

# Run database migrations
npm run typeorm migration:run

# Start the application in watch mode
npm run start:dev
