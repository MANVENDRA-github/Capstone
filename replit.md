# Mind Matters - Mental Health Platform

## Overview

Mind Matters is a comprehensive mental health support platform that connects users with licensed therapists and provides 24/7 AI-powered mental health assistance. The platform serves three primary user types: patients seeking mental health support, licensed therapists providing professional services, and administrators managing the platform. The system features real-time chat capabilities, appointment scheduling, mental health assessments, and a robust therapist verification system.

## User Preferences

Preferred communication style: Simple, everyday language.

## System Architecture

### Frontend Architecture
The client-side application is built with React and TypeScript, utilizing a modern component-based architecture. The UI is constructed using shadcn/ui components with Radix UI primitives, providing accessible and customizable interface elements. The design system follows healthcare-inspired aesthetics with a calming color palette featuring soft teal and lavender tones, implementing both light and dark themes.

State management is handled through React's built-in hooks and context, with TanStack Query managing server state and API interactions. The routing system uses Wouter for lightweight client-side navigation between authentication flows, dashboards, and chat interfaces.

### Backend Architecture
The server implements a RESTful API using Express.js with TypeScript. The application follows a layered architecture with clear separation between routes, business logic, and data access layers. A storage interface pattern abstracts database operations, making the system database-agnostic while providing type-safe CRUD operations.

Session management is implemented using express-session with PostgreSQL session storage, ensuring secure user authentication and maintaining session state across requests.

### Database Design
The system uses PostgreSQL with Drizzle ORM for type-safe database operations. The schema supports multi-role user management with a base users table and specialized therapist profiles. Core entities include:

- Users with role-based permissions (user, therapist, admin)
- Therapist profiles with licensing, credentials, and specialization data
- Chat sessions and messages for real-time communication
- Mental health assessments for tracking user progress
- Session storage for authentication state

The database design enforces referential integrity and supports the platform's multi-tenant architecture where therapists can manage multiple clients.

### Authentication & Authorization
The platform integrates with Replit Auth for streamlined user authentication, supporting both regular users and licensed professionals. The system implements role-based access control, ensuring therapists can only access their assigned clients and users can only view their own data.

User registration flows differ based on role - therapists undergo additional verification including license validation, credential verification, and professional background checks.

### Real-time Communication
Chat functionality is implemented with support for both AI-powered conversations and human therapist interactions. The system maintains chat session history and supports different conversation types including crisis intervention, general support, and scheduled therapy sessions.

### AI Integration
The platform includes an intelligent chatbot for 24/7 mental health support, designed to provide immediate assistance while recognizing when human intervention is necessary. The AI system includes mental health assessments and can escalate critical situations to human therapists.

## External Dependencies

### Database & ORM
- **PostgreSQL**: Primary database via Neon Database serverless platform
- **Drizzle ORM**: Type-safe database operations and schema management
- **connect-pg-simple**: Session storage in PostgreSQL

### UI & Design System
- **Radix UI**: Accessible component primitives for forms, dialogs, and navigation
- **shadcn/ui**: Pre-built component library with customizable design tokens
- **Tailwind CSS**: Utility-first styling with custom design system variables
- **Lucide React**: Icon library for consistent visual elements

### Authentication & Session Management
- **Replit Auth**: Primary authentication provider with social login support
- **express-session**: Server-side session management with PostgreSQL storage

### Development & Build Tools
- **Vite**: Frontend build tool with hot module replacement
- **TypeScript**: Type safety across frontend and backend
- **ESBuild**: Server-side bundling for production deployment

### State Management & API
- **TanStack Query**: Server state management and caching
- **React Hook Form**: Form validation and submission handling
- **Zod**: Runtime schema validation and type inference

### Utilities & Enhancement
- **date-fns**: Date manipulation and formatting
- **nanoid**: Unique identifier generation
- **class-variance-authority**: Type-safe CSS class variant management
- **clsx & tailwind-merge**: Conditional CSS class composition