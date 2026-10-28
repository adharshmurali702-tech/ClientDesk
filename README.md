# ClientDesk

A responsive freelancer workspace built with HTML, CSS and JavaScript.

## Run
Open dist/index.html in your browser. No Python or package installation required. For consistent storage, use a static local server or the hosted site.

## Features
- Overview with computed revenue, active projects and upcoming deadlines
- Create, edit, search and delete clients
- Project board with editable stages, budgets and deadlines
- Single-line invoices with unique numbers, manual payment status and print-to-PDF
- Revenue reports based on payment dates
- Local storage, JSON backups and validated restore
- Light/dark appearance and responsive layout

Demo records are explicitly labeled. Clear them in Settings to start your own workspace. Data lives in the current browser, not in a cloud account. Download backups regularly. Email sending, payment processing, multi-user accounts and a shared client portal are not implemented.

## Project structure
- dist/index.html: accessible application shell and editor dialog
- dist/style.css: responsive design system, themes and invoice print layout
- dist/app.js: application state, forms, rendering and persistence
- checks.cjs: render/data smoke checks using the Node standard library

Run checks with `node checks.cjs` and syntax validation with `node --check dist/app.js`.

Google Fonts are optional: local sans-serif fallbacks remain available offline.

## Portfolio learning tasks
Trace a client edit through the form, state and localStorage. Explain how the overdue invoice status is derived. Add invoice line items and tax calculations, then replace local storage with authenticated server storage to support a client portal.
