# 🎓 Campus Circle

### A Social Networking and Event Management Platform for University Communities

Campus Circle is a full-stack web application designed specifically for university students, faculty, and administrators. It provides a centralized digital platform for campus communication, social interaction, event discovery, and community engagement.

The platform combines social networking features with campus event management to reduce fragmented communication and create a connected university community.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Problem Statement](#-problem-statement)
- [Solution](#-solution)
- [Objectives](#-objectives)
- [Key Features](#-key-features)
- [User Roles](#-user-roles)
- [Technology Stack](#-technology-stack)
- [System Architecture](#-system-architecture)
- [Application Workflow](#-application-workflow)
- [Project Structure](#-project-structure)
- [Authentication & Security](#-authentication--security)
- [Database](#-database)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Future Enhancements](#-future-enhancements)
- [Project Benefits](#-project-benefits)
- [Contributors](#-contributors)
- [License](#-license)

---

# 📖 Overview

Campus Circle is a university-focused social platform that brings students, faculty, clubs, and administrators together in one centralized application.

Traditional campus communication is often distributed across multiple platforms such as messaging groups, email, notice boards, and social media. This makes it difficult for students to discover events, follow campus activities, and interact with their university community.

Campus Circle addresses this problem by providing a dedicated platform for:

- Social interaction
- Campus announcements
- Events
- Event registration
- Student networking
- Content sharing
- Notifications
- Role-based campus management

The application follows a full-stack architecture with a React-based frontend, Node.js/Express backend, and MongoDB database.

---

# ❗ Problem Statement

University students often face difficulties in accessing campus information because communication is fragmented across different platforms.

Common problems include:

- Important announcements being missed
- Events being communicated through multiple channels
- Difficulty discovering campus activities
- Limited interaction between students and faculty
- No centralized student community
- Difficulty managing event registrations
- Lack of personalized campus content
- Information being scattered across different applications

Campus Circle aims to provide a single platform that addresses these challenges.

---

# 💡 Solution

Campus Circle provides a centralized social and event-management platform where university users can:

1. Create and manage profiles
2. Share posts
3. Like and comment on posts
4. Follow other users
5. Save useful posts
6. Discover campus events
7. Create and manage events
8. RSVP to events
9. Receive notifications
10. Interact according to their assigned role

This creates a connected digital campus environment.

---

# 🎯 Objectives

The major objectives of Campus Circle are:

- Create a centralized university community platform
- Improve communication between students and faculty
- Simplify campus event discovery and registration
- Provide social networking features for students
- Implement secure authentication
- Support role-based access control
- Provide personalized social feeds
- Improve student engagement with campus activities
- Build a scalable full-stack web application

---

# 🚀 Key Features

## 👤 User Authentication

Campus Circle provides secure authentication for users.

Features include:

- User registration
- User login
- University email verification
- JWT-based authentication
- Secure sessions
- Logout functionality
- Protected routes

---

## 🔐 Role-Based Access Control

Different users have different permissions.

Supported roles include:

### Student

Students can:

- Create profiles
- View the social feed
- Create posts
- Like posts
- Comment on posts
- Save posts
- Follow other users
- Discover events
- RSVP to events
- Receive notifications

### Faculty

Faculty members can participate in the campus community and interact with students and campus activities according to their assigned permissions.

### Admin

Administrators can manage platform-level activities and maintain the campus community.

---

# 📰 Social Feed

The social feed allows users to interact with the university community.

Users can:

- Create posts
- View posts
- Like posts
- Comment on posts
- Save posts
- Follow users
- View personalized content

The feed provides a centralized place for campus-related communication and social interaction.

---

# ❤️ Likes and Comments

Users can interact with posts using:

- Likes
- Comments
- Saved posts

These features encourage student engagement and community interaction.

---

# 👥 Follow System

Users can follow other members of the campus community.

The follow system helps users create a personalized network and discover content from people they are interested in.

---

# 📅 Event Management

Campus Circle includes an event management system.

Users can:

- Discover upcoming events
- View event information
- Check event details
- RSVP to events
- Track their participation

Authorized users can also create and manage campus events.

---

# 🔔 Notifications

The notification system helps users stay updated about important activities.

Notifications can be used for:

- Social interactions
- Event updates
- RSVP-related updates
- Campus activities
- Other important platform events

---

# 🎨 User Interface

The frontend is designed to provide a modern and responsive experience.

The interface focuses on:

- Simple navigation
- Responsive layouts
- Clean components
- Easy access to campus information
- Social feed interaction
- Event discovery
- User profiles

The application is designed to work across different screen sizes.

---

# 🛠️ Technology Stack

## Frontend

- React.js
- JavaScript
- Tailwind CSS
- HTML5
- CSS3

## Backend

- Node.js
- Express.js
- REST APIs

## Database

- MongoDB

## Authentication

- JWT (JSON Web Tokens)
- University email verification
- Role-Based Access Control

## Development Tools

- Git
- GitHub
- VS Code
- npm

---

# 🏗️ System Architecture

Campus Circle follows a full-stack client-server architecture.

```text
                ┌──────────────────────┐
                │      User / Client   │
                │  Student / Faculty   │
                │       / Admin        │
                └──────────┬───────────┘
                           │
                           ▼
                ┌──────────────────────┐
                │   React Frontend     │
                │                      │
                │  UI Components       │
                │  Pages               │
                │  Forms               │
                │  Event UI            │
                │  Social Feed         │
                └──────────┬───────────┘
                           │
                       REST APIs
                           │
                           ▼
                ┌──────────────────────┐
                │ Node.js + Express    │
                │      Backend         │
                │                      │
                │ Authentication       │
                │ Authorization        │
                │ Business Logic       │
                │ Event Management     │
                │ Social Features      │
                └──────────┬───────────┘
                           │
                           ▼
                ┌──────────────────────┐
                │      MongoDB         │
                │                      │
                │ Users                │
                │ Posts                │
                │ Comments             │
                │ Events               │
                │ RSVPs                │
                │ Notifications        │
                └──────────────────────┘
