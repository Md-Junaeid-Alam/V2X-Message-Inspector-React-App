# V2X Message Inspector & Fleet Console

> 🚧 **Status: Work in Progress** — this project is under active development. Features, architecture, and UI are evolving as it's built out phase by phase.

A React-based tool for inspecting, filtering, and analyzing simulated V2X (Vehicle-to-Everything) messages — Basic Safety Messages (BSMs), misbehavior reports, and signal phase messages — in a live, interactive console. Think of it as a lightweight "Wireshark for V2X," built to explore message streams, flag anomalies, and visualize fleet-wide risk in real time.

This project is being built as a hands-on way to demonstrate practical React proficiency (hooks, state architecture, performance patterns, custom hooks, routing, testing) within a real automotive/V2X domain context, alongside related work on [VehicleLink Gateway](https://github.com/Md-Junaeid-Alam/VehicleLink-Gateway).

## Planned Features

- [ ] Simulated V2X message stream (BSMs, misbehavior reports, signal phase messages)
- [ ] Live message feed with filtering and flagging
- [ ] Intersection/map view showing vehicle positions and status
- [ ] Per-vehicle detail view with message history
- [ ] Risk/anomaly scoring and analytics dashboard
- [ ] Scenario builder for injecting custom vehicles and anomalies

## Tech Stack

- **React** + **Vite**
- **React Router** for navigation (`/`, `/vehicle/:id`, `/analytics`)
- **Zustand** for live fleet/message state
- **TanStack Query** for any async/server-derived data
- **TypeScript** (in progress)
- **Vitest** + **React Testing Library** for testing

## Project Structure

```
src/
  app/          # composition root: App.jsx, routes, providers
  features/     # feature-based modules (console, vehicle-detail, analytics)
  shared/       # reusable components and hooks
  store/        # Zustand stores
  main.jsx
  index.css
```

## Getting Started

```bash
npm install
npm run dev
```

## Roadmap

This project is being developed incrementally across several phases, covering core React fundamentals through advanced patterns (custom hooks, performance optimization, testing, and TypeScript). Commit history reflects this phased approach.

---

*Part of an ongoing portfolio of V2X/automotive cybersecurity projects, alongside [VehicleLink Gateway](https://github.com/Md-Junaeid-Alam/VehicleLink-Gateway).*
