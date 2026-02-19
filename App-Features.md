Lab 1 – App Features (TS.5.3)

## Core Features

- **User Authentication:** Sign up, log in, password reset, and secure sessions.
- **Lesson Browser:** Browse, search, and filter available lessons and modules.
- **Lesson Viewer:** View lesson content including text, images, video, and embedded code examples.
- **Progress Tracking:** Track completed lessons, percentage progress, and resume where left off.
- **Interactive Exercises:** Quizzes and coding exercises with automated feedback and scoring.
- **Admin Content Management:** Create, edit, and publish lessons; manage users and permissions.

## System Needs

- **Persistent Database:** A reliable database (e.g., PostgreSQL or MongoDB) for users, lessons, progress, and results; include backup strategy.
- **Authentication & Security:** Secure authentication (JWT/OAuth2), password hashing, HTTPS, and session management.
- **Media Storage & CDN:** Scalable file storage for lesson media (e.g., AWS S3) and CDN for fast content delivery.
- **RESTful API / Frontend:** Versioned API endpoints and a responsive frontend app (SPA) to consume them.
- **Logging & Monitoring:** Application logging, error tracking, and performance monitoring (e.g., Sentry, Prometheus).

## Notes

This document supports Lab 1 (TS.5.3). Instructors may adapt feature scope for each cohort.
