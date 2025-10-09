FitCRM – Simple Client Manager for a Fitness Program
====================================================

A lightweight, frontend-only CRM web app to help fitness professionals manage basic client information and track fitness goals. Built with semantic HTML and modern CSS (Flexbox/Grid), designed to work well on both desktop and mobile.

Note: This is a static prototype. Buttons and actions are placeholders and do not persist data.


Overview
--------
- **Project Type**: Frontend-only (HTML + CSS)
- **Target Users**: Fitness instructors, personal trainers, small gym owners
- **Purpose**: Provide a simple interface to add a new client (form page) and view a list of clients (table page) with mock actions


Live Demo and Repository
------------------------
- **Live App**: [Add your deployed URL here]
- **GitHub Repository**: [Add your public GitHub repo URL here]


Features (Functional Requirements)
----------------------------------
1) New Client Form (Page 1)
   - Full Name (text)
   - Age (number)
   - Gender (dropdown)
   - Email (email input)
   - Phone (tel)
   - Fitness Goal (dropdown or free text)
   - Membership Start Date (date)
   - “Add Client” button (placeholder – no persistence)

2) Client List View (Page 2)
   - Table showing 10 sample clients
   - Columns: Name, Email, Phone, Fitness Goal, Membership Start Date
   - Row actions: Edit, Delete (placeholders)
   - Search box to filter by client name (UI only in this prototype)

3) Responsive Design
   - Layout built with CSS Flexbox/Grid
   - Scales for desktop and mobile
   - Optional media queries for enhanced responsiveness


Tech Stack
----------
- **HTML5** for structure
- **CSS3** (Flexbox/Grid, media queries) for layout and responsiveness
- No JavaScript or backend included in this prototype


Project Structure
-----------------
```
fitcrm/
├── index.html
├── css/
│   └── styles.css
├── assets/
│   └── icons/
│       ├── delete.svg
│       ├── edit.svg
│       ├── logo.svg
│       └── search.svg
└── README.md
```


Getting Started (Local)
-----------------------
No build tools are required.

1. Clone or download this repository.
2. Open `index.html` directly in your browser.
   - On Windows, you can double‑click `index.html` or right‑click → Open With → your browser.


Pages
-----
- `index.html` includes the markup for:
  - New Client Form section
  - Client List View section with sample data and placeholder actions
  - A search box above the table (visual only in this prototype)

- `css/styles.css` contains all styles for layout, typography, color, and responsiveness.


Deployment
-----

```
https://faridafitcrm.netlify.app/

```
