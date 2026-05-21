# hrms-client — Human Resource Management System

A modern, enterprise-grade HR Management System frontend built with **Angular 17** and **Angular Material UI**.

---

## 🌐 Live Demo
> Coming Soon

## 🔗 Backend API Repository
> [HRMS Backend](https://github.com/YogeshKhatkale/HRMS)

---

## 🖼️ Screenshots

### Login Page
> Clean, professional login with demo credentials

### Dashboard
> Module cards with quick access to all HR features

### Sidebar Navigation
> Dark blue enterprise-style sidebar with all modules

---

## ⚡ Tech Stack

| Technology | Version | Purpose |
|---|---|---|
| Angular | 17+ | Frontend Framework |
| Angular Material | 21+ | UI Component Library |
| TypeScript | 5+ | Programming Language |
| SCSS | - | Styling |
| JWT | - | Authentication |
| RxJS | - | Reactive Programming |
| HTTP Client | - | API Communication |

---

## 📦 Modules

| Module | Status |
|---|---|
| ✅ Authentication (Login / Register) | Complete |
| ✅ Dashboard | Complete |
| ✅ Sidebar Navigation | Complete |
| ✅ Layout (Toolbar + Sidenav) | Complete |
| 🔄 Employee Management | In Progress |
| 🔄 Attendance Management | Coming Soon |
| 🔄 Leave Management | Coming Soon |
| 🔄 Payroll Management | Coming Soon |
| 🔄 Recruitment Management | Coming Soon |
| 🔄 Reports & Analytics | Coming Soon |

---

## 🏗️ Project Structure

```
src/
└── app/
    ├── core/
    │   ├── guards/
    │   │   └── auth-guard.ts         → Route protection
    │   ├── interceptors/
    │   │   └── jwt-interceptor.ts    → Attach JWT token to requests
    │   └── services/
    │       └── auth.ts               → Login, Register, Logout
    │
    ├── features/
    │   ├── auth/
    │   │   ├── login/                → Login page
    │   │   └── register/             → Register page
    │   ├── dashboard/                → Dashboard with module cards
    │   └── employees/
    │       └── employee-list/        → Employee list page
    │
    ├── shared/
    │   ├── layout/                   → Sidebar + Top toolbar layout
    │   ├── models/
    │   │   └── auth.models.ts        → TypeScript interfaces
    │   └── sidebar/                  → Sidebar component
    │
    ├── app.config.ts                 → App providers & interceptors
    ├── app.routes.ts                 → Application routing
    └── app.html                      → Root component template
```

---

## 🔐 Authentication Flow

```
User enters credentials
        ↓
Angular calls POST /api/Auth/login
        ↓
API returns JWT token
        ↓
Token stored in localStorage
        ↓
JWT Interceptor attaches token to every request
        ↓
Auth Guard protects private routes
        ↓
User redirected to Dashboard
```

---

## 🎨 UI Features

- ✅ Professional dark blue sidebar navigation
- ✅ Responsive layout with toggle sidebar
- ✅ Angular Material components throughout
- ✅ Azure/Blue Material theme
- ✅ Role badge display (Admin, HR, Manager, Employee)
- ✅ User profile in sidebar footer
- ✅ Notification bell in toolbar
- ✅ Gradient module cards on dashboard
- ✅ Custom favicon and browser title
- ✅ Login page with demo credentials

---

## 🚀 Getting Started

### Prerequisites

```
Node.js    → v18 or higher
Angular CLI → v17 or higher
npm        → v9 or higher
```

### Installation

```bash
# Clone the repository
git clone https://github.com/YogeshKhatkale/hrms-client.git

# Navigate into the project
cd hrms-client

# Install dependencies
npm install

# Start development server
ng serve
```

Open your browser at:
```
http://localhost:4200
```

### Demo Credentials

```
Email    → admin@hrms.com
Password → Admin@123
```

> Make sure the backend API is running at https://localhost:7099

---

## ⚙️ Environment Configuration

Update the API URL in:
```
src/app/core/services/auth.ts
```

```typescript
private apiUrl = 'https://localhost:7099/api/Auth';
```

For production, update to your Azure App Service URL.

---

## 🌍 Deployment

| Service | Platform | Cost |
|---|---|---|
| Frontend | Azure Static Web Apps | Free Forever |
| Backend API | Azure App Service F1 | Free Forever |
| Database | Azure SQL / Supabase | Free Tier |

### Deploy Frontend to Azure Static Web Apps

```bash
# Build for production
ng build --configuration production

# Deploy via GitHub Actions (auto on push to main)
```

---

## 🔗 Related Repositories

| Repository | Description |
|---|---|
| [HRMS Backend](https://github.com/YogeshKhatkale/HRMS) | ASP.NET Core 8 Web API |
| [hrms-client](https://github.com/YogeshKhatkale/hrms-client) | This repository |

---

## 📋 Roadmap

- [x] Login & Register pages
- [x] JWT Authentication
- [x] Dashboard with module cards
- [x] Sidebar navigation layout
- [ ] Employee Management (List, Create, Edit, Delete)
- [ ] Attendance tracking
- [ ] Leave management
- [ ] Payroll processing
- [ ] Recruitment pipeline
- [ ] Reports & Analytics
- [ ] Dark mode
- [ ] Mobile responsive
- [ ] Azure deployment

---

## 👨‍💻 Developer

**Yogesh Khatkale**

- 🐙 GitHub → [@YogeshKhatkale](https://github.com/YogeshKhatkale)
- 💼 Project → HRMS Full Stack Portfolio Project
- 🛠️ Stack → ASP.NET Core 8 + Angular 17 + SQL Server + Azure

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
