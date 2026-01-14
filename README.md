# IDURAR ERP/CRM

**IDURAR ERP/CRM** is a modern, full-stack **Enterprise Resource Planning (ERP)** and **Customer Relationship Management (CRM)** system designed to help businesses manage finance, customers, inventory, users, and reporting from a single, unified platform.

Built with a **React + Node.js + MongoDB** stack and fully containerized using  **Docker Compose** , IDURAR focuses on scalability, maintainability, and developer experience.

---

## 🚀 Key Capabilities

* End-to-end **business management**
* Modular and extensible architecture
* REST-based backend API
* Secure authentication and role-based access
* Production-ready Docker setup

---

## Screenshots

![1768379484197](image/README/1768379484197.png)

![1768379613871](image/README/1768379613871.png)

## 📌 Application Features

### 1️⃣ Financial Management

**Invoicing & Billing**

* Create, edit, and delete invoices
* Tax and discount calculation
* Multi-currency support
* PDF invoice generation
* Email invoice delivery
* Invoice status tracking

**Payments**

* Payment records and history
* Partial payments
* Payment receipts
* Manual payment tracking (gateway-agnostic)

**Expenses**

* Expense categorization
* Expense records
* Financial summaries

---

### 2️⃣ Customer Relationship Management (CRM)

* Customer profiles
* Contact information management
* Lead tracking
* Sales opportunities
* Deal pipeline
* Quote-to-invoice workflow
* Customer segmentation

---

### 3️⃣ Inventory & Products

* Product catalog
* Categories and variants
* Stock tracking
* Inventory valuation
* Low-stock indicators
* Product images
* Stock movement history

---

### 4️⃣ User & Access Management

* User accounts
* Role-Based Access Control (RBAC)
* Permission management
* Secure JWT authentication
* Profile management
* Activity protection via middleware

---

### 5️⃣ Reporting & Analytics

* Sales reports
* Financial reports
* Customer insights
* Product performance analytics
* Dashboard visualizations
* Exportable data (PDF-ready)

---

### 6️⃣ Document & File Management

* File uploads (invoices, receipts, assets)
* Secure file storage
* PDF generation
* Document downloads

---

### 7️⃣ Notifications & Integrations

* Email notifications (Resend)
* AI integrations (OpenAI)
* External service readiness
* REST API integration support

---

## 🧱 Tech Stack (Verified)

### Frontend

| Technology       | Version | Purpose          |
| ---------------- | ------- | ---------------- |
| React            | 18.3.1  | UI Library       |
| Redux Toolkit    | 2.2.1   | State Management |
| Ant Design       | 5.14.1  | UI Components    |
| Vite             | 5.4.8   | Build Tool       |
| React Router DOM | 6.22.0  | Routing          |
| Axios            | 1.6.2   | HTTP Client      |
| dayjs            | ^1.11.x | Date Handling    |
| react-quill      | ^2.x    | Rich Text Editor |

---

### Backend

| Technology | Version | Purpose            |
| ---------- | ------- | ------------------ |
| Node.js    | 20.9.0  | Runtime            |
| Express.js | 4.18.2  | REST API Framework |
| MongoDB    | 6.0     | Database           |
| Mongoose   | 8.1.1   | ODM                |
| JWT        | 9.0.2   | Authentication     |
| Multer     | 1.4.4   | File Uploads       |
| OpenAI SDK | 4.27.0  | AI Services        |
| Resend     | 2.0.0   | Email Delivery     |

---

### DevOps & Tooling

* Docker
* Docker Compose
* Git & GitHub
* Environment-based configuration
* ESLint & Prettier

---

## 🗂️ Project Structure

```
.
├── backend/        # Express API & business logic
├── frontend/       # React application
├── mongodb/        # MongoDB initialization & volumes
├── doc/            # Documentation
├── features/       # Feature definitions
├── docker-compose.yml
├── README.md
└── LICENSE
```

---

## 🐳 Docker Setup (Recommended)

### Prerequisites

* Docker
* Docker Compose

### Run the Application

```bash
docker-compose up -d --build
```

### Access Services

* Frontend: `http://localhost:3000`
* Backend API: `http://localhost:4000`
* MongoDB: `localhost:27017`

---

## 🧪 Local Development (Without Docker)

### Backend

```bash
cd backend
npm install
npm run dev
```

### Frontend

```bash
cd frontend
npm install
npm run dev
```

---

## 🔐 Environment Variables

### Backend (`.env`)

```
PORT=4000
MONGODB_URI=mongodb://localhost:27017/idurar
JWT_SECRET=your_secret_key
```

---

## 🔐 Security Highlights

* JWT-based authentication
* Secure password hashing
* Role-based authorization
* Input validation
* Controlled file uploads
* CORS protection

---

## 📊 Database Collections (Core)

* users
* roles
* customers
* leads
* invoices
* payments
* products
* inventory
* expenses

---

## 📈 Architecture Overview

```
Browser
   ↓
Frontend (React + Vite)
   ↓
Backend API (Express)
   ↓
MongoDB (Docker)
```

## 🧭 Roadmap Ideas

* WebSocket support
* Payment gateway integration
* Advanced reporting
* Audit logs
* Multi-tenant support

---

## 📜 License

This project is licensed under the  **MIT License** .

---

## ⭐ Final Note

**IDURAR ERP/CRM** is a robust, extensible foundation for building modern business management platforms.
It is suitable for  **SMBs, SaaS products, and enterprise prototypes** .
