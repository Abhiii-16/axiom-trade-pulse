# Token Trading Dashboard – Frontend Project

## Project Overview

This project is a **frontend token trading dashboard** built as part of a technical assignment focused on **pixel-accurate UI replication, performance optimization, and scalable component architecture**.

The application recreates a professional-grade token discovery table commonly used in crypto trading platforms. The primary goal was not just visual similarity, but also **production-level frontend practices**, including real-time data simulation, smooth micro-interactions, and reusable design patterns.

All functionality is implemented purely on the frontend, with mocked data streams to simulate live market behavior.

---

## Assignment Context

### Task Summary

The assignment required building a **token trading table interface** with the following expectations:

- Multiple token categories displayed simultaneously
- Rich interaction patterns (hover states, tooltips, sorting, modals)
- Real-time style updates using mocked streaming data
- Skeleton loading states and error handling
- Pixel-accurate UI with minimal layout deviation
- High performance with smooth animations and fast interactions

The solution was expected to follow modern frontend standards using **Next.js, TypeScript, Tailwind CSS**, and structured state management.

---

## How This Project Addresses the Task

### Token Table Structure
- Implemented three independent token sections (e.g. new listings, trending tokens, migrated tokens)
- Each section renders independently to avoid unnecessary re-renders
- Consistent column alignment across sections

### Interaction Design
- Hover-based row highlighting
- Click interactions for filtering and sorting
- Contextual tooltips for dense numeric data
- Modal-based advanced filtering

### Real-Time Simulation
- Mock WebSocket logic to simulate live token updates
- Distinct update frequencies per token category
- Smooth color transitions for price and metric changes

### Loading & Error States
- Skeleton placeholders that exactly match final layout dimensions
- Pre-allocated spacing to prevent layout shifts
- Graceful fallback for missing or broken token images

### Performance Considerations
- Memoized components for frequently updating UI
- Separation of UI state and async data state
- No unnecessary DOM updates during data refresh cycles

---

## Image & Avatar Handling

- Token logos are loaded dynamically via API-provided image URLs
- Images fade in smoothly once loaded
- Broken or unavailable images fall back to a symbol-based placeholder
- No hard dependency on local image assets, matching real-world trading dashboards

---

## Component Architecture

The project follows **Atomic Design principles** to ensure scalability and reuse.

