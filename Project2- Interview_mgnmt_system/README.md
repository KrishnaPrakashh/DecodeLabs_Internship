# Recruitment & Interview Management System

## Overview

The Recruitment & Interview Management System is a full-stack web application designed to streamline the recruitment process. The system allows candidates to apply for job positions, track their application status, and view interview schedules. HR personnel can manage applications, update candidate statuses, schedule interviews, and review candidate information.

This project demonstrates full-stack web development concepts including frontend development, backend API creation, routing, CRUD operations, and data management using Node.js and Express.js.

---

## Features

### Applicant Portal

* Apply for available job positions
* Submit personal information and candidate description
* Check application status using email address
* View interview schedule details
* Track recruitment progress

### HR Portal

* View all submitted applications
* Search candidates by name
* Review candidate details
* View candidate descriptions
* Update application status
* Schedule interviews
* Manage interview information

### Status Management

* Applied
* Shortlisted
* Interview Scheduled
* Selected
* Rejected

---

## Technologies Used

### Frontend

* HTML5
* CSS3
* Bootstrap 5
* JavaScript (ES6)

### Backend

* Node.js
* Express.js

### Data Storage

* JSON File Storage

  The application currently uses JavaScript data files for temporary storage:
  
  ```text
  data/
  ├── application.js
  └── interviews.js
  ```
  
  Data is maintained in memory during server execution, enabling simple CRUD operations without requiring a database.
  
  **Limitation:** Data is reset whenever the server restarts.
  
  **Future Enhancement:** Implement persistent storage using JSON files or MongoDB.
  

### Version Control

* Git
* GitHub

---

## Project Structure

```text
Recruitment-Interview-Management-System
│
├── applicant
│   ├── apply.html
│   ├── apply.js
│   ├── my_status.html
│   └── status.js
│
├── hr
│   ├── applications.html
│   ├── applications.js
│   ├── interviews.html
│   ├── interviews.js
│   ├── candidate_details.html
│   └── candidate_details.js
│
├── routes
│   ├── application.js
│   └── interview.js
│
├── data
│   ├── applications.js
│   └── interviews.js
│
├── index.html
├── style.css
├── server.js
├── package.json
└── README.md
```

---

## API Endpoints

### Applications

| Method | Endpoint                   | Description               |
| ------ | -------------------------- | ------------------------- |
| POST   | /apply                     | Submit application        |
| GET    | /applications              | Get all applications      |
| GET    | /application-status/:email | Get application by email  |
| PUT    | /applications/:id          | Update application status |

### Interviews

| Method | Endpoint                 | Description                     |
| ------ | ------------------------ | ------------------------------- |
| POST   | /interviews              | Schedule interview              |
| GET    | /interviews              | Get all interviews              |
| GET    | /interviews/:candidateId | Get candidate interview details |

---

## Installation

### Clone Repository

```bash
git clone <repository-url>
```

### Navigate to Project Folder

```bash
cd Recruitment-Interview-Management-System
```

### Install Dependencies

```bash
npm install
```

### Run Server

```bash
node server.js
```

### Open Application

```text
http://localhost:5000
```

---

## Workflow

### Candidate Workflow

1. Open the application.
2. Navigate to Apply for Job.
3. Submit application details.
4. Enter candidate description.
5. Check application status using email.
6. View interview details when scheduled.

### HR Workflow

1. Open HR Portal.
2. View submitted applications.
3. Search candidates.
4. Review candidate details.
5. Update application status.
6. Schedule interviews.
7. Manage recruitment process.

---

## Future Enhancements

* Database Integration (MongoDB/MySQL)
* Authentication and Authorization
* HR Login System
* Email Notifications
* Resume Upload Feature
* Interview Feedback Management
* Dashboard Analytics
* Candidate Profile Management

---

## Learning Outcomes

* REST API Development
* CRUD Operations
* Express.js Routing
* Client-Server Communication
* Bootstrap UI Development
* JavaScript DOM Manipulation
* Project Structure Organization
* Git and GitHub Version Control

---

## Author

Krishna Prakash

Full Stack Development Internship Project
