# 📋 TaskFlow - Enterprise Task Management System

[![Python](https://img.shields.io/badge/Python-3.12%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-6.1%2B-092E20?style=for-the-badge&logo=django&logoColor=white)](https://www.djangoproject.com/)
[![React](https://img.shields.io/badge/React-18%2B-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
[![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)
[![JWT](https://img.shields.io/badge/Auth-JWT-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white)](https://jwt.io/)
[![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)](LICENSE)

A full-stack, enterprise-grade Task Management System built with **React** and **Python Django**. Designed to streamline company task delegation, workflow management, and real-time tracking with strict Role-Based Access Control (RBAC), modern dynamic views (Kanban, Gantt chart, List/Grid Explorer), and secure JWT authentication.

---

## 💡 System Architecture & Design Philosophy

TaskFlow is architected around a **decoupled RESTful API architecture** separation between a React SPA client and a Django REST application backend.

```
┌─────────────────────────────────────────────────────────┐
│                       React SPA                         │
│   (React Router • Component Views • URL Filtering)      │
└────────────────────────────┬────────────────────────────┘
                             │ REST API (JSON / JWT)
┌────────────────────────────▼────────────────────────────┐
│                    Django Backend                       │
│    (Models • Serializers • Views • RBAC Middleware)     │
└────────────────────────────┬────────────────────────────┘
                             │ ORM
┌────────────────────────────▼────────────────────────────┐
│                   SQLite Database                       │
│       (Users • Roles • Tasks • Categories)             │
└─────────────────────────────────────────────────────────┘
```

### 🔒 Role-Based Access Control (RBAC) Matrix

Security and data access are strictly governed at both backend API and frontend routing levels:

| Role | Permissions & Capabilities |
| :--- | :--- |
| 🛡️ **Admin** | Superuser with full system rights. Can create, view, update, and delete any task across the enterprise, manage user roles, and access system configurations. |
| 👔 **Manager** | Operational supervisor. Can create new tasks, update, and view tasks assigned to them or created by their team. |
| 👷 **Worker** | Individual contributor. Can view tasks explicitly assigned to them and update task progress/completion status. |

---

## ✨ Features & Capabilities

- 🔄 **Full Task Lifecycle Management (CRUD)**: Create, detail view, edit, delete, and archive tasks.
- 📊 **Multiple Visual Views**:
  - **Kanban Board**: Drag-and-drop / status column workflow.
  - **Gantt Chart View**: Project timeline tracking and schedule overview.
  - **Explorer List & Grid View**: Filterable task table with multi-attribute sorting.
  - **Task Detail View**: Deep dive into task activity and metadata.
  - **Completed Archive**: Dedicated historical view for completed assignments.
- 🎯 **Advanced Filtering & Dynamic Routing**: Dynamic URL parameter sync for status (`Raised`, `Pending`, `Closed`), priority (`High`, `Medium`, `Low`), and category filtering.
- 🔐 **Stateless JWT Authentication**: Secure login session handling with refresh token rotation and client-side route protection.
- 📱 **Responsive UI & Dynamic Design System**: Mobile-first design system derived from modern UI mockups (`stitch` design system).
- ⏳ **UX Delighter Features**: Skeleton loading states, graceful error boundaries, and notifications.

---

## 🗃️ Task Data Schema

Each task within the system enforces structured metadata:

| Field Name | Type / Values | Description |
| :--- | :--- | :--- |
| `Task Header` | String | Concise title of the task |
| `Task Description` | Text | Detailed breakdown of requirements |
| `Priority` | Enum (`High`, `Medium`, `Low`) | Urgency level |
| `Category` | Enum (`Academic`, `Personal`, `Raised`) | Organizational classification |
| `Created At` | Timestamp | Automatically recorded timestamp |
| `Due Date` | Date (`DD/MM/YYYY`) | Target completion date |
| `Status` | Enum (`Raised`, `Pending`, `Closed`) | Current lifecycle state |
| `Assignees` | Many-to-Many | Workers/Managers assigned to execute the task |

---

## 🛠️ Tech Stack & Tooling

### **Frontend**
- **Library**: React 18+
- **Routing**: React Router DOM (v6+) with Protected Route Wrappers
- **UI Framework**: Custom Modular CSS & Component Design System (Stitch Mockups)
- **State & HTTP**: Context API / Hooks + Axios for REST API interaction

### **Backend**
- **Framework**: Python 3.12+ with Django 6.1+
- **API Engine**: Django REST Framework (DRF)
- **Authentication**: SimpleJWT / JSON Web Tokens
- **Database**: SQLite3 (Development / Production ready schema)
- **Dependency Management**: [`uv`](https://github.com/astral-sh/uv) fast Python package manager

---

## 📁 Project Structure

```
task_management_system/
├── backend/
│   ├── manage.py                          # Django management CLI
│   ├── task_management_system_project/    # Project settings & URL routing
│   └── task_management_system_app/        # Core app (Models, Views, Serializers, RBAC)
├── frontend/
│   └── stitch_react_task_management_system/
│       └── stitch_react_task_management_system/
│           ├── dashboard_overview/        # Main Kanban & summary dashboard
│           ├── tasks_explorer_list_grid/  # List & Grid Explorer view
│           ├── task_details_dynamic_route/# Dynamic task detail view
│           ├── add_new_task_form/         # Task creation & editing interface
│           └── completed_tasks_archive/   # Historical completed task archive
├── skills/
│   └── rules.md                           # System design & business rules specification
├── main.py                                # Entry wrapper script
├── pyproject.toml                         # Project metadata & dependencies (uv)
└── README.md                              # Showcase documentation
```

---

## 🚀 Getting Started

Follow these steps to set up and run the application locally.

### **Prerequisites**
- **Python**: 3.12 or higher
- **Node.js**: v18+ and `npm`
- **uv** (Optional but recommended): `pip install uv`

---

### **1. Backend Setup (Django REST API)**

```bash
# Navigate to the backend directory
cd backend

# Create and activate virtual environment using uv or standard venv
uv sync
# OR
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate

# Run database migrations
python manage.py migrate

# Create an Admin user (Superuser)
python manage.py createsuperuser

# Start the Django backend development server
python manage.py runserver
```
> The Django backend will be available at `http://127.0.0.1:8000/`.

---

### **2. Frontend Setup (React Application)**

```bash
# Navigate to the frontend directory
cd frontend/stitch_react_task_management_system/stitch_react_task_management_system

# Install dependencies
npm install

# Run the development server
npm start
# OR
npm run dev
```
> The React frontend application will launch at `http://localhost:3000/`.

---

## 🔌 API Endpoints (Quick Reference)

| Method | Endpoint | Description | Auth Required |
| :--- | :--- | :--- | :--- |
| `POST` | `/api/token/` | Obtain JWT access & refresh tokens | ❌ No |
| `POST` | `/api/token/refresh/` | Refresh expired access token | ❌ No |
| `GET` | `/api/tasks/` | List all tasks (filtered by user role & query parameters) | ✅ Yes |
| `POST` | `/api/tasks/` | Create a new task (Admin & Manager only) | ✅ Yes |
| `GET` | `/api/tasks/<id>/` | Retrieve specific task details | ✅ Yes |
| `PUT/PATCH` | `/api/tasks/<id>/` | Update task details / status | ✅ Yes |
| `DELETE` | `/api/tasks/<id>/` | Delete task (Admin only) | ✅ Yes |

---

## 🗺️ Future Enhancements

- [ ] **Google OAuth2 Integration**: Add social login support alongside local authentication.
- [ ] **Custom Analytics Dashboard**: Advanced telemetry and team velocity metrics.
- [ ] **Real-time Notifications**: WebSockets / Server-Sent Events for instant task updates.

---

## 📝 License

This project is open-source and available under the [MIT License](LICENSE).
