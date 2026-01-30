# EduManage
📌 Problem Statement
Many schools still rely on fragmented or manual systems to manage academic operations. Handling students, teachers, classes, attendance, and access control across multiple tools leads to inefficiency, data inconsistency, and security risks.
EduManage aims to provide a centralized, secure, and role-based platform that simplifies school administration and improves data accessibility for all stakeholders.


#Stakeholders

Admin – Manages users, classes, and overall system configuration

Teacher – Manages assigned classes, student attendance, and academic records

Student – Views personal profile, attendance, and academic information



#Core Requirements

Secure Authentication System using JWT and cookies

Role-Based Access Control (RBAC) to restrict features based on user roles

Class Management for assigning teachers and students

Attendance Tracking with date-wise records

Pagination & Search to efficiently handle large datasets


#system architecture


This project follows a three-tier architecture to ensure scalability, security, and maintainability.
Frontend — React.js
Built using React.js as a single-page application (SPA)

Handles user interface, client-side routing, and state management

Communicates with the backend via RESTful APIs

Uses Axios  for HTTP requests

Consumes and renders JSON responses



2. backend Django (REST Framework)
Developed using Django with Django REST Framework (DRF)

Manages business logic and API handling

Implements authentication and authorization

Uses serializers for data validation and transformation

Exposes RESTful endpoints for frontend consumption


3.database -SQL
Uses a relational SQL database ( SQLite)

Stores structured and relational application data

Ensures data integrity through constraints and indexing

Integrated with Django using Django ORM


Request Flow
User interacts with the React frontend

React sends an HTTP request to the Django REST API

Django processes the request and queries the SQL database

Database returns the data to Django

Django sends a JSON response back to React

React updates the UI dynamically



