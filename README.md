# Multi-Tenant SaaS Platform

A **production-ready, scalable multi-tenant SaaS application** designed for managing projects and tasks with **strict tenant isolation**, **secure authentication**, and **role-based access control**.  
The system is fully containerized and can be launched using a **single Docker Compose command**.

---

## 🚀 Key Features

- Complete tenant data isolation  
- JWT-based secure authentication  
- Role-Based Access Control (RBAC) with three roles:
  - `super_admin`
  - `tenant_admin`
  - `user`
- End-to-end project and task management  
- Automated database migrations and seed data execution  
- Containerized backend, frontend, and database services  
- Dedicated backend health-check endpoint  

---

## 🛠️ Technology Stack

### Backend
- Node.js  
- Express.js  
- PostgreSQL  
- JWT Authentication  
- Role-Based Access Control (RBAC)  

### Frontend
- React (Vite)  
- Axios for API communication  
- Role-based UI rendering  

### Infrastructure & Deployment
- Docker  
- Docker Compose  

---

## ▶️ Getting Started

### Start the Application
From the project root directory, run:

```bash
docker-compose up -d
