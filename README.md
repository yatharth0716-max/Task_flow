# Welcome to your Lovable project

# Team Task Manager

A real-time, full-stack team task management application designed to support collaborative workflows, role-based access, and modern SaaS-level user experience.
Built using React, Vite, Tailwind CSS, and Supabase.

---

## Live Demo

https://nudge-team.lovable.app

---

## Overview

This project implements a scalable task management system with real-time synchronization, granular permissions, and team collaboration features. It is designed to simulate a production SaaS environment where multiple users can manage tasks, track progress, and collaborate efficiently.

---

## Core Features

### Dashboard

* Displays key metrics: total, completed, in-progress, and overdue tasks
* Visual analytics using charts for task distribution and weekly productivity
* “My Tasks Today” section for quick access
* Real-time activity feed
* Project progress tracking

---

### Task Management

* Kanban board with drag-and-drop (Todo, In Progress, Done)
* Inline task creation with keyboard shortcut support
* Priority-based color coding
* Search and filtering options
* Overdue task indicators
* Optimistic UI updates for smooth interaction

---

### Teams and Roles

* Team creation and joining via invite links or codes
* Role-based access control (Admin, Member)
* Member management with role switching and ownership transfer
* Confirmation workflows for critical actions

---

### Collaboration

* Threaded comments on tasks
* File attachments with secure access
* Task-level activity tracking
* Deadline reminders and scheduling
* Granular task-level permissions (view, comment, edit, admin)

---

### Notifications

* Real-time notifications for task and team updates
* Notification panel with unread indicators
* Ability to mark notifications as read

---

### User Experience

* Dark mode with modern design system
* Fully responsive layout
* Sidebar navigation with collapse support
* Focus mode for distraction-free usage
* Smooth animations and loading states

---

## Architecture

### Frontend

* React (Vite) with TypeScript
* Tailwind CSS and component-based design
* React Query for data fetching
* Drag-and-drop using @hello-pangea/dnd
* Charts using Recharts

---

### Backend

* Supabase (PostgreSQL, Authentication, Realtime)
* Row Level Security (RLS) for data protection
* Edge Functions for background jobs and reminders

---

## Database Design

The system uses a relational schema with the following key entities:

* Users and profiles
* Teams and memberships
* Tasks with status, priority, and assignments
* Activities and notifications
* Comments and attachments
* Task-level permissions and reminders

Granular access control is implemented using database-level security policies and helper functions. 

---

## Real-Time Capabilities

* Task updates reflected instantly across users
* Live notifications and activity tracking
* Real-time collaboration on comments, attachments, and task changes

---

## Security

* Row Level Security ensures users only access authorized data
* Role-based authorization for team and task operations
* Secure file storage with controlled access

---

## Setup Instructions

### Clone the repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

### Install dependencies

```bash
npm install
```

### Configure environment variables

Create a `.env` file:

```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_key
```

---

### Run the application

```bash
npm run dev
```

Open in browser: http://localhost:5173

---

## Project Highlights

* Real-time multi-user collaboration system
* Fine-grained permission control at both team and task levels
* Scalable backend architecture using Supabase
* Modern, responsive UI inspired by industry tools
* Designed with production-level considerations

---

## Future Enhancements

* Calendar-based task visualization
* Integration with external tools (email, messaging platforms)
* Advanced analytics and reporting
* AI-assisted task recommendations

---

## License

This project is licensed under the MIT License.

