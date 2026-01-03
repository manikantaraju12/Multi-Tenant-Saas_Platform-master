# Multi-Tenant SaaS Platform

A **production-ready, scalable multi-tenant SaaS application** designed for managing projects and tasks with **strict tenant isolation**, **secure authentication**, and **role-based access control**.  
The system is fully containerized and can be launched using a **single Docker Compose command**.

---

## Key Features

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

## Technology Stack

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

### Getting Started
### Start the Application

- From the project root directory, run:
- docker-compose up -d
- Verify Backend Health
- After starting the services, verify that the backend is running correctly:
- curl http://localhost:5000/api/health
- Access the Application
- Web UI: http://localhost:3000

No manual database setup is required.
Database schema creation and seed data are handled automatically on application startup.

---

### Service Endpoints
Service	URL:
- Frontend	http://localhost:3000
- Backend API	http://localhost:5000
- Health Check	http://localhost:5000/api/health

---

### Preloaded Evaluation Credentials
Tenant Administrator
-Email: admin@acet.com
-Password: Admin@123
-Tenant ID: acet
These credentials are also documented in submission.json.

---

### Login Instructions
- Navigate to: http://localhost:3000/login
- Enter the provided credentials
- Submit the login form
- You will be redirected to the main dashboard
- With this account, you can:
- Manage users and roles
- Create and maintain projects
- Assign and track tasks
- Perform tenant-level administrative actions

---

### Authentication & Authorization Model
- Role	Permissions
- super_admin	Full system-wide control
- tenant_admin	Administrative control within a tenant
- user	Standard tenant-level access
Each tenant operates in complete isolation from all other tenants.

---

### Dockerized Services & Ports
Service	Description	Port Mapping
- database	PostgreSQL database	5432 → 5432
- backend	Express API server	5000 → 5000
- frontend	React web application	3000 → 3000

---

### Application Validation Checklist
-After launching the application:
- Access the frontend interface
-Authenticate using seeded credentials

---

### Verify:

- Tenant-level data isolation
- Role-based access permissions
- Project and task workflows

---
  

### Demonstration Video
The demo walkthrough includes:

- System architecture overview
- Docker-based deployment process
- Tenant isolation demonstration
- User, project, and task operations

---

### Demo reference :
https://drive.google.com/file/d/19-I6o1B8UJIXyF1PfAJmPYbNrVQXAOih/view

---

### Information for Evaluators
- Fully containerized SaaS implementation
- Single-command startup using Docker Compos
- Automated database initialization
- No manual configuration required

---

 ### Project Summary
This project demonstrates a real-world multi-tenant SaaS architecture built using modern backend and frontend technologies.
It emphasizes secure tenant isolation, role-based authorization, and automated database lifecycle management.
All services run independently and are orchestrated using Docker Compose, following industry-standard design practices.
