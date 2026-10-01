# Task Management System

## Intro

I am building a task management system to help me keep track of a company's daily tasks and to-dos. It is a simple application that allows me to add, update, delete, and view tasks. It also allows me to mark tasks as completed and incomplete. It also has diffent way to view task. Gnatt chart, kanban dashboard, list view etc. Task can be assigned to different users and each user can have different roles and permissions. User can be assigned to multiple tasks and each task can be assigned to multiple users. An authentication system is also implemented to secure the application. After logging in, the user is redirected to the dashboard. Authorization system is also implemented. Here **Admin** is the super user with all the permissions. There is also **Manager** role with limited permissions. And the least powerful role is **Worker** role with very limited permissions. Admin can create, update, delete and view any task. Manager can only update and view tasks assigned to them or the tasks they created. Worker can only view tasks assigned to them and update their status.  

## Features

* Add tasks: Allows me to add new tasks to the system.
* Update tasks: Allows me to update existing tasks.
* Delete tasks: Allows me to delete tasks.
* View tasks: Allows me to view all tasks.
* Mark tasks as completed: Allows me to mark tasks as completed.
* Mark tasks as incomplete: Allows me to mark tasks as incomplete.
* URL Parameters: Use URL parameters to filter and sort tasks.
* Navigation: Use React Router to navigate between pages.
* Protected Routing: All routes should be protected and should only be accessible to authenticated users.
* Loading States: Show loading states while fetching data from the backend.
* Error Handling: Handle errors gracefully and show appropriate messages to the user.
* UI Consistency: Maintain a consistent UI design throughout the application.
* Mobile Responsiveness: The application should be responsive and work on different screen sizes.
* Performance: The application should be performant and should not have any performance issues.
* Accessibility: The application should be accessible to users with disabilities.
* Login: 
* Logout: 
* Protected Dashboard:
* JWT Token: Remember user for a certain period of time.

## High Level Tasks
1. Build the UI of the application using React, the design is created using stitch and is inside the `./frontend/stitch_react_task_management_system/stitch_react_task_management_system` folder, here you will find multiple folders with code and screen of each individual pages. These pages are example of how the final UI should look like, it does not contain all the features of the application. You can use these pages as a reference to build the UI of the application.
2. Build the backend of the application using Django. Make multiple models as needed, multiple serializer as needed, multiple views as needed, multiple urls as needed, multiple APIs as needed. Create the backend within the backend within the backend folder in `./backend`. Here the django project is `backend/task_management_system_project` and application is `./backend/task_management_system_app`.
3. Connect the UI to the backend.
4. Connect the backend to the SQLite Database.

## Tasks Feature
Each task has the following fields:  
- Task Header  
- Task Description  
- Priority: High/Medium/Low 
- Category: Academic/Personal/ Raised 
- Date and Time: Automatically picked 
- Due Date: DD/MM/YYYY
- Status: Raised / Pending/Closed 


## Tech Stack

* Frontend: React
* Backend: Python Django Application
* Database: SQLite

## Rules
1. All files should be well-documented.
2. All files should be well-formatted.
3. All files should be well-commented.
4. All files should be well-structured.
5. All files should be well-named.
6. All files should be well-tested.
7. All files should be well-documented.
8. All files should be well-formatted.
9. All files should be well-commented.
10. All files should be well-structured.
11. All files should be well-named.
12. All files should be well-tested.
13. Don't delete anything without my permission.
14. Don't change the architecture of the application without my permission.

## Future
1. Keep Google Login as place holder in sign up/login page. As of now it will only have local login using email and password.
2. Currently custom admin panel is not required. we can implement django admin panel.

## Directory Architecture
* All the submodules will be in their dedicated folders. 

'''
my-project-root/                 # Main repository root directory
├── .gitignore                   # Ignores node_modules, venv, .env, etc.
├── README.md
│
├── backend/                     # ALL DJANGO BACKEND CODE
│   ├── manage.py                # Django CLI tool
│   ├── requirements.txt         # Python dependencies
│   │
│   ├── myproject/               # Project configuration app
│   │   ├── __init__.py
│   │   ├── asgi.py
│   │   ├── settings.py          # Database and API configurations
│   │   ├── urls.py              # Main URL routing (points to api/ urls)
│   │   └── wsgi.py
│   │
│   └── api/                     # Core API application (can break into more apps if large)
│       ├── migrations/
│       ├── __init__.py
│       ├── admin.py
│       ├── apps.py
│       ├── models.py            # Database schemas
│       ├── urls.py              # API endpoint routes (/api/v1/...)
│       ├── views.py             # Request logic (or use a views/ folder)
│       └── serializers.py       # Converts models to JSON for React
│
└── frontend/                    # ALL REACT FRONTEND CODE (Vite or Create-React-App)
    ├── package.json             # NPM dependencies & scripts
    ├── vite.config.js           # Or webpack.config.js / next.config.js
    ├── index.html               # The entry HTML file where React mounts
    │
    ├── public/                  # Unbundled static assets (favicons, robots.txt)
    └── src/                     # Core React codebase
        ├── main.jsx             # App entry point (mounts to DOM)
        ├── App.jsx              # Core layout component / Router wrapper
        ├── index.css            # Global styles
        │
        ├── assets/              # Shared static media (images, svgs, logos)
        ├── components/          # Reusable UI elements (Buttons, Navbar, Modals)
        ├── context/             # React Context / State Management files
        ├── hooks/               # Custom React hooks (e.g., useAuth)
        ├── services/            # API call modules (Axios/Fetch configs)
        └── pages/               # Full page views (Home, Login, Dashboard)
'''