# RecipeCart

A cross-platform recipe and shopping list application built with React Native and Expo.

The project focuses on simplifying meal planning, grocery shopping, and recipe management by combining recipes, shopping workflows, product organization, and collaboration features into a single mobile-first experience.

One of the main goals was designing an application that feels practical for everyday use while maintaining scalable architecture and smooth cross-platform performance across iOS, Android, and web.

The project also served as hands-on experience in building larger React Native applications with Firebase-backed real-time data workflows, modular architecture, and modern mobile UX patterns.

---

## Features

### Recipe Management
- Create, edit, and organize recipes
- Recipe photos, ingredients, and step-by-step instructions
- Recipe filtering and categorization

### Recipe Extraction
- Import recipes directly from URLs
- In-app browser based recipe extraction workflow

### Shopping Lists
- Generate shopping lists automatically from recipes
- Manual shopping list creation
- Drag-and-drop item reordering

### Barcode Scanner
- Scan product barcodes
- Add products into a shared product catalog

### Product Catalog
- 25 predefined product categories
- Custom categories per shared library

### Shared Libraries
- Collaborate on recipe libraries with other users
- Invite-based library sharing

### Shopping List Sharing
- Share lists via links
- Export shopping lists as formatted text

### Mobile UX Features
- Dark / light mode support
- Haptic feedback integration
- Mobile-first interactions and navigation

### Localization
- English and Finnish language support

---

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | React Native + Expo |
| Language | TypeScript |
| Backend | Firebase (Firestore, Storage, Auth) |
| Navigation | React Navigation |
| Animations | React Native Reanimated + Gesture Handler |
| State Management | React Context |
| Localization | i18next |
| Testing | Jest + Testing Library |

---

## Architecture & Focus Areas

The project focuses heavily on:
- scalable React Native architecture
- cross-platform mobile development
- reusable component structure
- real-time Firebase workflows
- maintainable state management
- mobile UX and interaction design

Special attention was given to keeping business logic separated from UI components through:
- custom hooks
- service-layer architecture
- typed Firebase service abstractions

This helped keep screens lightweight and maintainable as the application grew in complexity.

---

## Key Design Decisions

### Service Layer Isolation
All Firebase reads and writes go through typed service modules instead of directly accessing Firebase from UI screens.

### Custom Hooks
Business logic was extracted into reusable hooks to keep components focused on presentation and user interaction.

### Shared Recipe Libraries
Recipe libraries were designed to support collaboration between multiple users with shared access and custom category systems.

### Dynamic Category System
Built-in and custom categories are merged dynamically to support flexible product organization workflows.

### Theme System
Theming architecture was designed for efficient runtime theme switching and consistent styling across the application.

---

## Challenges & Learnings

Some of the most challenging parts of the project included:

- Designing scalable Firebase data structures
- Building reusable mobile UI patterns
- Managing shared real-time data safely
- Handling complex shopping list workflows
- Designing maintainable React Native architecture
- Building smooth cross-platform UX behavior

The project significantly improved my understanding of:
- React Native architecture
- Firebase and real-time data handling
- mobile-first UX design
- scalable frontend structure
- TypeScript in larger applications
- AI-assisted software development workflows

---

## Development Workflow

Modern AI-assisted development workflows were actively utilized during development, including:
- GitHub Copilot
- Claude Code
- LLM-assisted prototyping and debugging

The goal was not only to accelerate development, but also to improve experimentation, architecture iteration, and problem-solving workflows.

---

## Testing

The project includes automated tests covering:
- UI components
- hooks
- business logic
- application workflows

Testing stack:
- Jest
- jest-expo
- React Native Testing Library

---

## Status

Private project – public source code not available.
