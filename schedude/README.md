# ScheDude

A mobile scheduling assistant designed to solve a simple but surprisingly common problem:

Most calendar apps tell you when your event starts.  
ScheDude tells you when you actually need to leave.

The application works backwards from event timing by combining:
- travel duration
- preparation time
- scheduled transit departures
- and the user’s own lateness patterns

to determine the real moment the user should stop what they are doing and start preparing.

Built with React Native for iOS and Android, the app combines behavioral insights, scheduling logic, notifications, and personality-driven UX into a more human approach to time management.

One of the core ideas behind the project was exploring how software can adapt to real human behavior instead of assuming users always act optimally.

---

## Core Concept

ScheDude does not simply notify users when an event starts.

Instead, it calculates:
- when to start preparing
- when to leave
- and how much behavioral buffer is realistically needed

based on historical user behavior and context.

The app also features a sarcastic animated blob character whose mood and behavior escalate as departure time approaches.

---

## Features

## Smart Departure Timing

### Dynamic Leave Time Calculation
Calculates departure timing using:
- event start time
- travel duration
- preparation time
- scheduled transit departures
- personalized lateness buffers

### Escalating Schedule States
The app transitions through four behavioral states:
- Calm
- Prepare
- Urgent
- Late

UI styling, colors, messaging, and character behavior adapt dynamically to each state.

---

## Behavioral Learning

### Personalized Buffer Logic
The app tracks whether users arrive:
- early
- on time
- late

A recency-weighted algorithm analyzes historical behavior and automatically adjusts future departure buffers.

### Adaptive Timing
Users who are consistently late gradually receive larger automatic timing buffers without manual configuration.

### Manual Override
Users can disable adaptive behavior and use fixed custom buffers instead.

---

## Notifications

### Preparation Reminders
The app sends reminders when it is time to begin preparing.

### Leave Alerts
Critical notifications fire when it is time to leave.

### Dynamic Rescheduling
Notifications automatically update when event details change.

---

## Post-Event Feedback Loop

After each event, users can log:
- whether they arrived on time
- how late they were
- or whether they arrived early

This data feeds back into the behavioral insights engine to improve future recommendations.

---

## Personal Insights

The “Me” section includes:
- on-time streak tracking
- lateness statistics
- behavioral insights
- customizable essentials checklist
  - keys
  - wallet
  - phone
  - etc.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | React Native |
| Language | TypeScript |
| State Management | Zustand + AsyncStorage |
| Navigation | React Navigation |
| Notifications | Notifee |
| Date Handling | Day.js |
| Graphics | react-native-svg |

---

## Architecture & Focus Areas

The project focuses heavily on:
- mobile-first UX
- behavioral product design
- scheduling logic
- local persistence
- reactive UI states
- state-driven interaction design

Special attention was given to separating:
- timing logic
- behavioral analysis
- notification orchestration
- UI state management

into maintainable and testable modules.

---

## Key Technical Decisions

### Pure Scheduling Logic
Timing calculations were isolated into standalone pure functions to simplify testing and maintainability.

### Behavioral Insights Engine
A recency-weighted analysis engine dynamically computes user lateness patterns and adjusts timing recommendations automatically.

### State-Driven UI
The entire UI reacts to scheduling urgency levels, including:
- colors
- animations
- messaging tone
- character behavior

### Local-First Persistence
User preferences, scheduling history, and insights persist locally for responsiveness and offline reliability.

---

## Scheduling Logic

The application calculates scheduling timing using formulas such as:

prepAt = leaveAt − prepMins

leaveAt = eventStart − travelMins − bufferMins

The behavioral buffer is automatically adjusted using recency-weighted lateness analysis:

smartBufferBonusMins = clamp(round(weightedAvgDelay × 0.75), 0, 20)

The system requires multiple resolved events before adaptive timing activates.

---

## Challenges & Learnings

Some of the most challenging parts of the project included:

- Designing behavioral timing algorithms
- Balancing helpfulness without becoming annoying
- Building reactive UI behavior tied to scheduling urgency
- Structuring maintainable mobile state management
- Coordinating notifications with dynamic scheduling logic
- Designing UX around real human habits instead of idealized behavior

The project significantly improved my understanding of:
- React Native architecture
- behavioral product design
- state-driven UI systems
- mobile scheduling workflows
- local persistence strategies
- user-centered mobile UX

---

## Development Workflow

The project was developed using modern AI-assisted development workflows, including:
- GitHub Copilot
- Claude Code
- LLM-assisted ideation and prototyping

AI tooling was primarily used to accelerate experimentation, architecture iteration, and rapid product exploration.

---

## Status

Personal side project — actively developed and evolving.
Not yet released publicly.
