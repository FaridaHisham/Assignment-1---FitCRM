# FitCRM – Client Management System for Fitness Professionals

<div align="center">

**A modern, lightweight CRM web application designed specifically for fitness professionals to manage client information, track fitness goals, and plan training sessions.**

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

</div>

---

## 📋 Table of Contents

- [Overview](#-overview)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Project Structure](#-project-structure)
- [Usage Guide](#-usage-guide)
- [Data Validation](#-data-validation)
- [Deployment](#-deployment)
- [Browser Support](#-browser-support)
- [Future Enhancements](#-future-enhancements)
- [License](#-license)

---

## 🎯 Overview

FitCRM is a fully functional client management system built for fitness instructors, personal trainers, and gym owners. It provides an intuitive interface to manage client information, track membership dates, set fitness goals, and plan workout sessions with exercises from the Wger API.

**Key Highlights:**
- ✅ **Fully Functional** - Complete CRUD operations with localStorage persistence
- ✅ **Smart Validation** - Comprehensive form validation including date validation
- ✅ **Responsive Design** - Beautiful UI that works seamlessly on desktop, tablet, and mobile
- ✅ **API Integration** - Fetches real exercise data from Wger Workout Manager API
- ✅ **No Backend Required** - Pure frontend application using browser localStorage

---

## ✨ Features

### 1. **Client Management**
- **Add New Clients** with comprehensive information:
  - Full Name, Age, Gender
  - Email and Phone contact details
  - Fitness Goal (predefined or custom)
  - Membership Start Date and End Date
- **Edit Existing Clients** - Update client information anytime
- **Delete Clients** - Remove clients with confirmation prompt
- **View Client Details** - Dedicated page showing full client profile

### 2. **Smart Search & Filtering**
- Real-time search by client name
- Instant table filtering
- Keyboard shortcuts (Enter to search, Escape to clear)

### 3. **Data Validation**
- **Email Validation** - Must end in `.com` or `.edu`
- **Phone Validation** - Exactly 11 digits required
- **Age Validation** - Between 5 and 120 years
- **Date Validation**:
  - Membership Start Date cannot be in the past
  - Membership End Date must be after Start Date

### 4. **Exercise Planning**
- Integration with **Wger Workout Manager API**
- Automatically suggests 5 random exercises for client sessions
- English-only exercise names for clarity
- Displays exercises with clean, modern UI

### 5. **Data Persistence**
- All client data stored in browser's **localStorage**
- Data persists across browser sessions
- No server or database required

### 6. **Responsive Design**
- Mobile-first approach
- Optimized layouts for:
  - 📱 Mobile phones (< 480px)
  - 📱 Tablets (481px - 768px)
  - 💻 Desktops (> 769px)
- Touch-friendly interface
- Smooth scrolling and animations

---

## 🛠 Tech Stack

| Technology | Purpose |
|------------|---------|
| **HTML5** | Semantic structure and accessibility |
| **CSS3** | Modern styling with Flexbox & Grid |
| **JavaScript (ES6+)** | Client-side logic and interactivity |
| **localStorage API** | Client-side data persistence |
| **Wger API** | Exercise database integration |

**Design Features:**
- Pastel purple theme with gradient accents
- Glassmorphism effects
- Smooth transitions and hover states
- Custom form styling with focus states

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No installation or build tools required!

### Local Setup

1. **Clone or Download** the repository:
   ```bash
   git clone https://github.com/yourusername/fitcrm.git
   cd fitcrm
   ```

2. **Open the application**:
   - Simply double-click `index.html`, or
   - Right-click `index.html` → Open With → Your Browser, or
   - Use a local server (optional):
     ```bash
     # Python 3
     python -m http.server 8000
     
     # Node.js (with http-server)
     npx http-server
     ```

3. **Start using FitCRM!**
   - Navigate to `http://localhost:8000` if using a local server
   - Or just open the file directly in your browser

---

## 📁 Project Structure

```
FitCRM/
├── index.html              # Main HTML file with all pages
├── css/
│   └── styles.css          # Complete styling and responsive design
├── js/
│   └── main.js             # Application logic and API integration
├── assets/
│   └── icons/
│       ├── delete.svg      # Delete action icon
│       ├── edit.svg        # Edit action icon
│       ├── logo.svg        # FitCRM brand logo
│       └── search.svg      # Search icon
└── README.md               # This file
```

---

## 📖 Usage Guide

### Adding a New Client

1. Click **"New Client"** from the navigation or home page
2. Fill in all required fields:
   - Full Name, Age, Gender
   - Email (must end in .com or .edu)
   - Phone (exactly 11 digits)
   - Fitness Goal (select from dropdown or enter custom)
   - Membership Start Date (today or future)
   - Membership End Date (must be after start date)
3. Click **"Add Client"** button
4. Client will be saved and appear in the Client List

### Viewing Client Details

1. Navigate to **"Client List"**
2. Click the **"View"** button next to any client
3. See complete client information
4. View suggested exercises for next training session
5. Click **"Edit This Client"** to make changes

### Editing a Client

1. From the Client List, click the **Edit** icon (pencil)
2. Form will populate with existing data
3. Make your changes
4. Click **"Save Changes"**
5. Click **"Cancel Edit"** to discard changes

### Deleting a Client

1. From the Client List, click the **Delete** icon (trash)
2. Confirm deletion in the popup
3. Client will be permanently removed from localStorage

### Searching Clients

1. Navigate to **"Client List"**
2. Type client name in the search box
3. Press **Enter** or click **"Search"**
4. Press **Escape** to clear search and show all clients

---

## ✅ Data Validation

FitCRM includes comprehensive validation to ensure data integrity:

| Field | Validation Rules |
|-------|------------------|
| **Full Name** | Required |
| **Age** | Optional, but if provided must be 5-120 |
| **Gender** | Required, dropdown selection |
| **Email** | Required, must end in `.com` or `.edu` |
| **Phone** | Required, exactly 11 digits |
| **Fitness Goal** | Required, dropdown or custom text |
| **Start Date** | Required, cannot be in the past |
| **End Date** | Required, must be after Start Date |

**Error Messages:**
- Clear, user-friendly alerts guide users to correct input
- Validation happens on form submission
- Prevents invalid data from being saved

---

## 🌐 Deployment

### Option 1: GitHub Pages

1. Push your code to a GitHub repository (must be public)
2. Go to repository **Settings** → **Pages**
3. Under **Source**, select branch (e.g., `main`) and folder (`/root`)
4. Click **Save**
5. Your site will be live at: `https://yourusername.github.io/fitcrm/`

### Option 2: Netlify

1. Go to [netlify.com](https://www.netlify.com) and sign up
2. Click **"Add New Site"** → **"Import an Existing Project"**
3. Connect your GitHub account and select your repository
4. **Build settings:**
   - Build command: (leave empty)
   - Publish directory: `/` (root)
5. Click **Deploy**
6. Your site will be live with a custom Netlify URL


I Deployed using Netflify my deployed webapp is on this link : https://faridafitcrm.netlify.app/
