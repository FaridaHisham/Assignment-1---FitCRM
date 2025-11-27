# FitCRM - Simple Client Manager for Fitness Programs

## Project Description

FitCRM is a lightweight client relationship management (CRM) web application built for fitness professionals like personal trainers, fitness instructors, and small gym owners. The app helps manage basic client information, track fitness goals, and plan workout sessions. This is a frontend-only project that uses browser localStorage for data persistence, so no backend server is needed.

This project was developed as part of CSCE 4502 - Design of Web-based Systems (Fall 2025), Assignment #2, building upon the foundation established in Assignment 1.

## Tech Stack

- **HTML5** - Structure and semantic markup
- **CSS3** - Styling with Flexbox/Grid for responsive layouts
- **JavaScript (ES6+)** - Client-side logic and interactivity
- **localStorage API** - Browser-based data persistence
- **Wger Workout Manager API** - External REST API for fetching exercise data

## Live Demo

**Deployed App:** https://faridafitcrm.netlify.app/

**GitHub Repository:** https://github.com/FaridaHisham/Assignment-1---FitCRM

## Features

### Page 1: New Client Form
- Add new clients with the following information:
  - Full Name
  - Age and Gender
  - Email and Phone
  - Fitness Goal (predefined options or custom)
  - Membership Start Date and End Date
- Form validation for all fields
- Data saved to localStorage when "Add Client" button is clicked

### Page 2: Client List View
- Display all clients in a table format
- **Search** - Find clients by name
- **View** - Click on a client to see their full details (goes to Page 3)
- **Edit** - Update client information (form repopulates with existing data)
- **Delete** - Remove client from list with confirmation prompt
- All changes persist in localStorage

### Page 3: Client View
- Display complete client information:
  - Name, Email, Phone
  - Fitness Goal
  - Membership Start Date and End Date
  - Training history
  - Suggested exercises for next session
- Fetches 5 random exercises from the Wger API for workout planning
- Option to edit client directly from this page

## Form Validation

The app includes validation to ensure data quality:
- **Email** - Must end in `.com` or `.edu`
- **Phone** - Must be exactly 11 digits
- **Age** - Must be between 5 and 120 (if provided)
- **Membership Start Date** - Cannot be in the past
- **Membership End Date** - Must be after the start date
- All required fields must be filled before submission

## Responsive Design

The app is fully responsive and works well on:
- Desktop computers
- Tablets
- Mobile phones

CSS Flexbox and Grid are used for flexible layouts, and media queries ensure the interface adapts to different screen sizes.

## Project Structure

```
fitcrm/
├── index.html              # Main HTML file containing all pages
├── css/
│   └── styles.css          # All styling and responsive design
├── js/
│   └── main.js             # JavaScript logic and API integration
├── assets/
│   └── icons/              # SVG icons for UI elements
│       ├── delete.svg
│       ├── edit.svg
│       ├── logo.svg
│       └── search.svg
└── README.md               # This file
```

## How to Run Locally

If you want to run the project on your local machine:

1. Clone or download this repository
2. Open the `index.html` file in any modern web browser (Chrome, Firefox, Safari, Edge)
3. That's it! No build process or dependencies to install.

Alternatively, you can use a local server:
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js http-server
npx http-server
```

Then navigate to `http://localhost:8000` in your browser.

## Deployment Method

This project is deployed on **Netlify**. The deployment process was straightforward:

1. Created a GitHub repository with the project code
2. Connected the repository to Netlify
3. Configured build settings (no build command needed since it's a static site)
4. Set publish directory to `/` (root)
5. Deployed automatically

The app is now live and accessible at: https://faridafitcrm.netlify.app/

## Data Persistence

All client data is stored in the browser's localStorage, which means:
- Data persists even after closing the browser
- No server or database required
- Data is stored locally on each user's device
- Clearing browser data will remove all stored clients

## API Integration

The app integrates with the **Wger Workout Manager API** to fetch exercise suggestions:
- API Documentation: https://wger.de/en/software/api
- Fetches 5 random exercises for each client's training session
- Filters for English-language exercises only
- Displays exercise names in a clean, readable format
  
**Assignment:** #2  
**Student:** Farida Hisham
