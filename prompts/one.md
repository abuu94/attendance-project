## From ChatGPT to be used in Lovable

# Build a Complete Frontend for an Attendance & Meeting Management System

Create a modern, professional, production-ready web application frontend for a Meeting and Attendance Management System used by EGaz (Zanzibar E-Government Authority).

The frontend will connect to an existing Django REST Framework (DRF) backend via REST APIs.

## Technology Requirements

Use:

* React
* Vite
* TypeScript
* TailwindCSS
* shadcn/ui
* React Router
* Axios
* React Hook Form
* TanStack Table
* Lucide React Icons

Use modern frontend best practices and a scalable feature-based architecture.

---

# User Roles

1. Super Admin
2. Admin
3. Public Attendee

---

# Core Business Workflow

The system manages meetings, meeting schedules, attendee registrations, token generation, and attendance verification.

Workflow:

1. Admin creates a Meeting
2. Admin creates Meeting Days under a Meeting
3. Public users register for a Meeting
4. Admin generates Meeting Tokens for each Meeting Day
5. Attendees receive a token
6. Attendees submit the token through the Attendance Confirmation page
7. System verifies attendance
8. Attendance records and token usage statistics are updated

---

# Main Modules

## Authentication

Pages:

* Login

Features:

* JWT Authentication
* Protected Routes
* Logout

---

## Dashboard

Create a modern analytics dashboard with:

Summary Cards:

* Total Meetings
* Total Meeting Days
* Total Registrations
* Total Attendance Confirmations
* Total Tokens
* Used Tokens
* Unused Tokens

Charts:

* Registrations by Meeting
* Attendance by Meeting
* Token Usage Overview

Recent Activity Section

---

## Meetings Management

Pages:

* Meetings List
* Create Meeting
* Edit Meeting
* Meeting Details

Features:

* Search
* Pagination
* Status Indicators
* Responsive Data Tables

---

## Meeting Days Management

Pages:

* Meeting Days List
* Create Meeting Day
* Edit Meeting Day

Features:

* Meeting Association
* Attendance Verification Toggle
* Filtering

---

## Registration Management

Pages:

* Registrations List
* Registration Details

Display:

* Full Name
* Institution
* Position
* Phone Number
* Email
* Bank Name
* Bank Account Number

Features:

* Search
* Filtering
* Pagination

---

## Meeting Tokens Management

Pages:

* Tokens List
* Token Details

Display:

* Token Value
* Used Status
* Used By
* Used At

Features:

* Token Statistics
* Status Badges
* Search and Filtering

---

## Attendance Management

Pages:

* Attendance Records
* Attendance Analytics

Display:

* Registration
* Meeting Day
* Token
* Confirmation Date

---

## Public Registration

Pages:

* Registration Form
* Registration Success Page

Features:

* Responsive Form
* Validation
* Professional User Experience

---

## Public Attendance Confirmation

Pages:

* Attendance Confirmation Form
* Success State
* Error State

Features:

* Token Submission
* Validation Feedback
* User-Friendly Messaging

---

# Backend Analytics Endpoints Available

Dashboard Summary:

GET /api/admin/dashboard/

Meetings Summary:

GET /api/admin/meetings/summary/

Single Meeting Summary:

GET /api/admin/meetings/{meeting_id}/summary/

Use these endpoints to power dashboard cards and charts.

---

# Design Requirements

Create a modern government-grade SaaS dashboard.

Design Style:

* Clean
* Professional
* Trustworthy
* Enterprise-grade

Color Palette:

* Blue
* Indigo
* Slate
* White

Layout:

* Collapsible Sidebar
* Top Navigation Bar
* Responsive Mobile Navigation

Components:

* Reusable Cards
* Tables
* Dialogs
* Forms
* Charts
* Status Badges

Provide:

* Responsive layouts
* Empty states
* Loading states
* Error states
* Toast notifications

---

# Architecture Requirements

Generate a scalable React project architecture using:

* Feature-based modules
* Reusable components
* Typed API services
* Centralized Axios instance
* Route protection
* Clean folder structure

Prepare the frontend for seamless integration with a Django REST Framework backend.

Focus on clean code, maintainability, scalability, and production readiness.
