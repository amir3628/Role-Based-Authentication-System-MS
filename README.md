# 🤖 Project Name – Role-Based Authentication System

A secure authentication and authorization system designed to enforce single active session per user, support login override, and maintain detailed audit logs. Built with scalability and security best practices in mind.

---
## Problem Statement

Modern applications often lack proper session control, allowing users to log in from multiple devices simultaneously, which increases security risks and reduces accountability. Additionally, insufficient logging makes it difficult to audit user activity or investigate incidents.

## ✅ Solution

This system enforces single-session login, provides a controlled override mechanism, and records all authentication-related events in audit logs, ensuring security, traceability, and compliance.

## ✨ Key Features
- Role-based authentication (Admin / User)
- Single active session per user
- Login override with confirmation
- Secure JWT-based authentication
- Redis-backed session management
- Detailed audit logs for all login activities
- Session termination on logout, timeout, or override

## 🛠 Tech Stack
- Backend: Node.js, Express.js
- Auth: JWT
- Session Store: Redis
- Database: MySQL
- Frontend (optional): React.js

## 🏗 Architecture Overview
Client → Auth API → JWT
              ↓
           Redis (Active Sessions)
              ↓
           MySQL (Users, Roles, Audit Logs)


## 🧬 Architecture
