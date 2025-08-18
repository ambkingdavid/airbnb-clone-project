# Overview
The Airbnb Clone Project is a full-stack backend simulation of a real-world booking platform. It focuses on building scalable backend architecture, designing relational databases, implementing secure APIs, and deploying with CI/CD pipelines.
# Project Goals
- Build a robust backend for a booking platform
- Practice collaborative development workflows
- Apply modern security and deployment practices
- Integrate Django, MySQL, and GraphQL into a unified system
# Team Roles
- Backend Developer:	Builds RESTful APIs, handles business logic, and integrates services
- Database Administrator:	Designs and manages the relational database schema and optimizes queries
- DevOps Engineer:	Sets up CI/CD pipelines, manages Docker containers, and automates deployments
- Security Specialist:	Implements authentication, authorization, and monitors for vulnerabilities
# Technology Stack
- Django: Web framework for building scalable APIs
- MySQL: Relational database for storing structured data
- GraphQL: Query language for flexible and efficient data retrieval
- Docker: Containerization for consistent development and deployment environments
- GitHub Actions: CI/CD automation for testing and deployment
# Database Design
Entities and Fields
- Users: id, name, email, password, created_at
- Properties: id, owner_id, title, location, price
- Bookings: id, user_id, property_id, start_date, end_date
- Reviews: id, user_id, property_id, rating, comment
- Payments: id, booking_id, amount, status, payment_date

Relationships
- One user can own multiple properties
- A booking belongs to one user and one property
- A property can have many reviews
- Each booking has one payment record
# Feature Breakdown
User Management Users can sign up, log in, and manage their profiles securely.
Property Management Hosts can list, edit, and delete properties with detailed descriptions and pricing.
Booking System Users can search for properties and make reservations based on availability.
Review System Guests can leave feedback and ratings for properties they’ve stayed in.
Payment Integration Secure payment processing for bookings using encrypted transactions.
# API Security
Authentication Use JWT tokens to verify user identity and maintain session integrity.
Authorization Role-based access control ensures users can only perform permitted actions.
Rate Limiting Prevents abuse by limiting the number of requests per user/IP.
Data Encryption Sensitive data like passwords and payment info are encrypted in transit and at rest.
# CI/CD Pipeline
CI/CD pipelines automate testing and deployment to ensure fast, reliable updates.
Continuous Integration (CI) Automatically runs tests on every commit using GitHub Actions.
Continuous Deployment (CD) Deploys code to production using Docker containers and GitHub workflows.
