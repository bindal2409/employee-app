# EmpView – Employee Management Portal
A fully functional ReactJS single-page application built as part of a ReactJS assignment. The app connects to a REST API to display employee data across multiple screens with camera capture, data visualization, and map integration.

---

## 🚀 Live Demo
Open `employee-app.html` directly in any browser or run with VS Code Live Server.

---

## 📋 Assignment Requirements Covered

| Requirement | Status |
|---|---|
| Login Page with authentication | ✅ Done |
| List Page with REST API data | ✅ Done |
| Details Page with camera capture | ✅ Done |
| Photo Result Page | ✅ Done |
| Bar Graph of employee salaries | ✅ Done |
| Map showing employee cities | ✅ Done |

---

## 📱 Screens

### 1. 🔐 Login Page
- Takes username and password as input
- Valid credentials: `testuser` / `Test123`
- Shows error message on wrong credentials
- Clean dark themed UI with gradient accents

### 2. 📋 Employee List Page
- Fetches data from the REST API on login
- Displays employees in a clean table format
- **Search bar** to filter across all fields
- **Pagination** — 10 employees per page
- **Stats cards** showing total employees, cities, departments, total payroll
- Click any row to go to Details page
- Buttons to navigate to Bar Graph and Map screens

### 3. 👤 Employee Details Page
- Shows all details of the selected employee
- Hero card with name and salary highlight
- Grid layout of all employee fields
- **Camera capture section** to take a photo

### 4. 📸 Photo Result Page
- Displays the photo captured from the camera
- Shows employee name and timestamp
- **Download button** to save the photo locally

### 5. 📊 Bar Graph Page
- Pure SVG bar chart (no external chart library)
- Plots salaries of the first 10 employees
- Color coded bars per employee
- Hover tooltips showing full name and salary
- Legend row below the chart

### 6. 🗺 Map Page
- Google Maps embed showing employee cities
- City pills showing employee count per city

---

## 🛠 Tech Stack

| Technology | Usage |
|---|---|
| ReactJS 18 | UI components and state management |
| Babel (in-browser) | JSX transpilation |
| Pure SVG | Bar chart (no external lib) |
| Google Maps Embed | City map |
| HTML5 Camera API | Photo capture via getUserMedia |
| CSS3 Animations | Fade-up, spin, pulse effects |
| Google Fonts | Syne + DM Sans typography |

---

## 📁 Project Structure

```
employee-app/
│
├── employee-app.html       ← Complete source code (single file)
├── README.md               ← This file
├── screenshots/
│   ├── login.png
│   ├── list.png
│   ├── details.png
│   ├── camera.png
│   ├── photo-result.png
│   ├── bar-graph.png
│   └── map.png
└── screen-recording.mp4    ← End-to-end demo
```

---

## ▶️ How to Run

### Option 1 — Direct Open
1. Download `employee-app.html`
2. Double-click to open in browser

### Option 2 — VS Code Live Server (Recommended)
1. Open `employee-app.html` in VS Code
2. Install the **Live Server** extension
3. Right-click → **"Open with Live Server"**
4. App opens at `http://127.0.0.1:5500`

---

## 🔌 REST API

| Property | Value |
|---|---|
| URL | `https://backend.jotish.in/backend_dev/gettabledata.php` |
| Method | POST |
| Body | `{"username": "test", "password": "123456"}` |

> **Note:** The API has CORS restrictions when called from localhost. The app automatically falls back to realistic mock data (20 employees) if the live API is unreachable, so all features remain fully functional for demonstration.

---

## 🎨 Design Highlights
- Dark theme with purple/pink gradient accents
- **Syne** display font + **DM Sans** body font
- Smooth fade-up animations on page transitions
- Noise texture overlay for depth
- Responsive layout with mobile support
- Sticky topbar with navigation
- Hover effects on all interactive elements

---

## 👤 Login Credentials
```
Username: testuser
Password: Test123
```

---

## 📌 Notes
- No build tools or npm required — runs directly in the browser
- All CSS, JavaScript, and React code is contained in a single HTML file
- Camera feature requires browser permission to access device camera
- Mock data includes 20 realistic Indian employee records as fallback
