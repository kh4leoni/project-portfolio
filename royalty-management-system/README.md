# Yoyalties

A fullstack royalty management system built for music labels to automate royalty tracking, reporting, recoup handling, and artist payout workflows.

The project was designed to simplify complex royalty operations by combining distributor report ingestion, royalty calculations, payout tracking, and PDF statement generation into a single platform.

One of the main goals was building a scalable and maintainable earnings engine capable of handling:
- royalty splits
- artist groups and member percentages
- recoup deductions
- payout tracking
- automated PDF statements

The project also served as hands-on experience in building larger fullstack applications with real-world business logic and PostgreSQL-backed architecture.

---

## Features

### Dashboard
- Revenue overview
- Monthly earnings chart with date filtering
- Top tracks and earners overview

### Report Ingestion
- Upload Excel distributor reports
- Duplicate detection using file hashing
- Automated report processing workflows

### Earnings Engine
- Per-artist royalty calculations
- Royalty split handling
- Distribution fee application
- Recoup expense deduction logic

### Artist Groups
- Support for bands and groups
- Configurable member split percentages
- Automatic payout distribution

### Payout Tracking
- Batch payout processing
- Full payout audit trail
- Earnings marked as paid automatically

### PDF Statements
- Generate artist payout statements
- Batch payout statement support

### Recoup Management
- Track advances and expenses
- Automatically apply deductions to future earnings

### Admin Tools
- Artist management
- Track management
- Royalty split management
- Distribution deal settings
- Auto-split workflows

### Authentication & Security
- Session-based authentication
- Rate limiting
- Timing-attack protection

---

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | Next.js (App Router) |
| Language | TypeScript |
| Database | PostgreSQL + Prisma ORM |
| Styling | Tailwind CSS |
| PDF Generation | PDFKit |
| Excel Parsing | xlsx |
| Authentication | bcryptjs + server-side sessions |
| Testing | Vitest |

---

## Architecture & Focus Areas

The project focuses heavily on:
- fullstack architecture
- backend business logic
- financial data handling
- relational database design
- maintainable API structure
- scalable calculation workflows

Special attention was given to keeping the royalty calculation logic modular and maintainable as payout and recoup workflows became more complex.

---

## Challenges & Learnings

Some of the most challenging parts of the project included:

- Designing flexible royalty split logic for both solo artists and groups
- Building recalculation workflows safely after data changes
- Structuring scalable payout and recoup pipelines
- Designing maintainable PostgreSQL schemas
- Handling complex financial logic reliably

The project significantly improved my understanding of:
- larger fullstack application architecture
- PostgreSQL and relational data modeling
- backend-focused business logic
- secure admin workflows
- AI-assisted software development workflows

---

## Development Workflow

Modern AI-assisted development workflows were actively utilized during development, including:
- GitHub Copilot
- Claude Code
- LLM-assisted prototyping and debugging

The goal was not only to speed up development, but also to improve experimentation, architecture iteration, and problem-solving workflows.

---

## Status

Private project – public source code not available.
