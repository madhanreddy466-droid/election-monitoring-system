# EMS — Election Monitoring System

A role-based, multi-portal election monitoring web application built with vanilla JavaScript. EMS lets citizens report issues, field observers log booth-level problems with photo evidence, analysts visualize trends, and admins manage everything from a central dashboard — all in a single responsive front-end app.

**Goal:** make election monitoring transparent and accessible, and help build a culture of informed civic participation among first-time voters.

## Features

- **Role-based access** — four distinct portals (Citizen, Observer, Analyst, Admin), each with its own navigation, permissions, and views
- **Citizen reporting** — submit election-related issues with optional photo evidence (client-side validation on file type and size)
- **Observer field reports** — log booth-level problems with up to 3 photo attachments and live report stats
- **Analyst dashboard** — interactive line, bar, and pie charts (ApexCharts) visualizing voting trends, report categories, and issue breakdowns, with keyword-based auto-categorization of incoming reports
- **Admin panel** — centralized view of all citizen issues, observer reports, and analyst notes, with status tracking, resolution workflow, and JSON export
- **Dark/light theme toggle** with a polished, responsive UI (custom CSS variables, glassmorphism cards, smooth transitions)

## Tech Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 |
| Styling | CSS3 (custom properties, gradients, responsive layout, dark/light themes) |
| Logic | JavaScript (ES6+, vanilla — no framework) |
| Charts | ApexCharts |
| Icons | Lucide |
| Data persistence | Browser `localStorage` (no backend — all state is client-side) |

## How to Run

1. Clone the repo:
   ```
   git clone https://github.com/madhanreddy466-droid/election-monitoring-system.git
   ```
2. Open `index.html` directly in any modern browser — no build step or server required.

## Key Learnings

- Designing a responsive, role-based interface with clean access control logic
- Managing real-time UI state and data flow using vanilla JavaScript and `localStorage`
- Building interactive data visualizations with ApexCharts
- Structuring a multi-portal single-page app without a framework

## Notes

This is a front-end-only project — all data (issues, reports, roles) is stored in the browser via `localStorage` and resets if browser storage is cleared. There is no backend or database.
