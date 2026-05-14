# Gainly

A full-stack digital coaching platform built for strength coaches and their clients.

Gainly was developed as part of a master’s thesis focused on AI-assisted software development workflows (“vibe coding”) and explores how modern LLM-assisted development impacts software architecture, development velocity, and product design in larger real-world applications.

The platform combines coaching workflows, workout tracking, messaging, progress analytics, and offline-first functionality into a single Progressive Web App designed for everyday use by both coaches and athletes.

One of the main goals of the project was building a production-grade application with:
- scalable architecture
- offline-first capabilities
- real-time communication
- role-based access control
- complex workout and PR tracking logic
- maintainable fullstack patterns

The project also served as hands-on experience in building larger systems using modern React, Next.js, Supabase, and AI-assisted development workflows.

---

## Features

## Coach Features

### Program Builder
- Drag-and-drop training program creation
- Week / block / day structure management
- Exercise configuration with reps, sets, and RPE targets

### Client Management
- Invite clients via secure email links
- View workout history and client progress
- Manage coach-client relationships

### Exercise Library
- Per-coach customizable exercise bank

### Messaging
- Real-time thread-based messaging between coach and client

---

## Client Features

### Workout Logger
- Log sets with weight, reps, and RPE
- Instant PR detection across multiple rep ranges
- Offline workout logging support

### Program View
- Weekly training schedule assigned by coach

### Progress Tracking
- Bodyweight tracking
- Waist measurements
- Strength progression charts
- Lift history visualization

### Offline-First Experience
- Works without network connection
- Automatic synchronization when online

---

## System Features

### Role-Based Security
- Row-level security enforced directly in PostgreSQL
- JWT-based role injection with Supabase auth hooks

### Real-Time Features
- Realtime messaging
- Live synchronization between users and devices

### PR Detection Engine
- Database-trigger-based personal record calculation
- Handles edits and deletions safely without stale records

### Progressive Web App
- Installable PWA
- Offline support
- Service worker caching strategies
- Mobile-friendly experience

---

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | Next.js + React |
| Language | TypeScript |
| Backend | Supabase (Postgres, Auth, Storage, Realtime) |
| Data Fetching | TanStack Query |
| Offline Storage | Dexie + IndexedDB |
| UI Components | Radix UI |
| Styling | Tailwind CSS |
| Forms | React Hook Form + Zod |
| Charts | Recharts |
| Drag & Drop | dnd-kit |
| Testing | Playwright + Vitest |

---

## Architecture & Focus Areas

The project focuses heavily on:
- scalable fullstack architecture
- offline-first application design
- real-time data synchronization
- role-based security
- maintainable React patterns
- database-driven business logic
- progressive web app architecture

Special attention was given to keeping the application maintainable as complexity increased through:
- typed query layers
- reusable UI architecture
- service abstraction patterns
- modular offline synchronization logic
- strict TypeScript configuration

The project also explores how AI-assisted development workflows can be integrated into larger production-oriented software projects.

---

## Key Technical Decisions

### Offline-First Workflows
Workout logging and client interactions were designed to function without internet connectivity using IndexedDB and background synchronization workflows.

### Database-Level Security
Authorization logic was intentionally enforced at the PostgreSQL layer using row-level security to minimize security risks in application code.

### Hybrid RSC + Client Architecture
Server Components handle data prefetching while client components consume hydrated query data for fast initial rendering.

### Trigger-Based PR Calculation
Personal record logic was implemented directly at the database level to ensure consistency even after edits and deletions.

### Role-Based Routing
JWT role claims are injected directly into authentication flows to support low-latency protected routing.

---

## Challenges & Learnings

Some of the most challenging parts of the project included:

- Designing reliable offline synchronization workflows
- Building scalable workout logging architecture
- Managing real-time data flows safely
- Implementing secure role-based access control
- Structuring larger PostgreSQL migration systems
- Balancing Server Components and client-side interactivity
- Designing maintainable application architecture as feature complexity increased

The project significantly improved my understanding of:
- large-scale React and Next.js architecture
- PostgreSQL and Supabase workflows
- offline-first application design
- real-time systems
- scalable TypeScript architecture
- progressive web applications
- AI-assisted software development workflows

---

## Development Workflow

The application was built using modern AI-assisted development workflows, with Claude Code acting as the primary development tool throughout the project.

AI tooling was utilized for:
- architecture iteration
- prototyping
- debugging
- implementation support
- workflow acceleration
- refactoring assistance

The project explored how LLM-assisted development affects:
- software architecture decisions
- development velocity
- maintainability
- developer workflows in larger real-world applications

---

## Testing

The project includes:
- end-to-end testing
- unit testing
- typed validation workflows
- database migration workflows

Testing stack:
- Playwright
- Vitest

---

## Status

Private project – public source code not available.
