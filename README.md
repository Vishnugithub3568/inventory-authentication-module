# Inventory Authentication Module

This repository contains the Authentication and Security module for the Inventory Monitoring and Reporting System.

The module implements secure user authentication using JSON Web Tokens (JWT) and role-based access control for employees and administrators.

## Features

- Secure user login
- JWT token generation and validation
- Password encryption
- Protected API routes
- Role-based authorization

## Project Structure

authentication/
Frontend authentication logic including login interface, token handling, and protected routes.

security/
Backend security implementation including JWT generation, authentication filters, and security configuration.

## Authentication Flow

1. User logs in using the LoginPage.
2. Credentials are sent to the backend AuthController.
3. System verifies the user using CustomUserDetailsService.
4. JwtUtil generates a JWT token.
5. Token is returned to the frontend.
6. ProtectedRoute ensures only authenticated users access protected pages.
7. JwtFilter validates the token for every backend request.

## Technologies Used

- Java (Spring Boot)
- JWT Authentication
- React / JavaScript
- GitHub for version control

## Purpose

This module ensures secure access to the Inventory Monitoring and Reporting System by validating user identity and protecting system APIs from unauthorized access.