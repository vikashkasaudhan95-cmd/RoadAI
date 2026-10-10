# RoadAI 🚧

### AI-Powered Road Hazard Detection & Alert System

**Know the road before you reach it.**

RoadAI is a road-safety project concept focused on community-powered hazard reporting and awareness. It explores a simple workflow:

**Report → Verify → Alert → Resolve**

The current implementation is a responsive front-end demo that lets visitors explore illustrative road-hazard reports,
add a demo report, filter reports, and change report statuses.

> **Current status:** Front-end demo / MVP concept. Sample locations and reports are illustrative,
>  and reports are stored in the current browser only. RoadAI is not an emergency service or an official live road-authority system.

## 📑 Table of Contents

- [Problem Statement](#-problem-statement)
- [Proposed Solution](#-proposed-solution)
- [Features](#-features)
- [Demo Workflow](#-demo-workflow)
- [Technology Stack](#-technology-stack)
- [Run Locally](#-run-locally)
- [Deploy with GitHub Pages](#-deploy-with-github-pages)
- [Project Structure](#-project-structure)
- [Future Scope](#-future-scope)
- [Safety, Privacy, and Limitations](#-safety-privacy-and-limitations)
- [Author](#-author)

## 🚨 Problem Statement

Road users may encounter potholes, waterlogging, debris, broken traffic signals, poor street lighting, and unsafe roadwork with little warning.

Information about these hazards can be scattered across messages, calls, and word of mouth. Without a structured reporting and tracking process,
it can be difficult to review reports, understand their current status, and make the resolution process more visible.

RoadAI explores a location-aware approach to organizing road-hazard reports and supporting better road-safety awareness.

## 💡 Proposed Solution

RoadAI is designed around four stages:

**Report → Verify → Alert → Resolve**

1. **Report:** Submit a hazard category, location or landmark, optional coordinates, and a short description.
2. **Verify:** Review report freshness, possible duplicates, and corroborating reports.
3. **Alert:** A future connected version could provide relevant proximity warnings designed to avoid distracting drivers.
4. **Resolve:** Track whether a report is new, corroborated, acknowledged, or resolved.


## ✨ Features

- Responsive dark navy and cyan dashboard.
- Summary cards for total reports, reports needing attention, high-severity reports, and resolved reports.
- Interactive map using Leaflet and OpenStreetMap tiles.
- Illustrative sample hazard markers around Kanpur.
- Hazard report form with category, severity, landmark, optional latitude and longitude, and description.
- Optional browser geolocation, subject to permission and secure-context requirements.
- Filters for all reports, reports needing attention, high-severity reports, and resolved reports.
- Demo actions to corroborate, resolve, reopen, and view a report on the map.
- Browser-local persistence using `localStorage`.
- Proposed technical architecture and future API integration plan.

## 🧪 Demo Workflow

1. Open the RoadAI website and explore the dashboard.
2. Review the illustrative hazard markers on the map.
3. Use the filters to narrow reports by status or severity.
4. Select **Report a hazard**.
5. Enter the required category, severity, and location or landmark.
6. Optionally enter both latitude and longitude, or use the location button after granting browser permission.
7. Submit the form to add a demo report.
8. Use the report actions to corroborate, resolve, reopen, or view the report on the map.
9. Select **Reset demo** to restore the illustrative sample reports.


## 🛠 Technology Stack

| Technology              | Purpose                                                         |
| ----------------------- | --------------------------------------------------------------- |
| HTML5                   | Website structure                                               |
| CSS3                    | Responsive layout and visual design                             |
| Vanilla JavaScript      | Form handling, filtering, report status updates, and demo logic |
| Leaflet                 | Interactive map                                                 |
| OpenStreetMap           | Map tiles and geographic display                                |
| Browser `localStorage`  | Saving demo reports in the current browser                      |
| Browser Geolocation API | Optional location capture                                       |

### Proposed Future Technologies

The following components are part of the proposed architecture and are not implemented in the current front-end demo.

| Technology                | Proposed purpose                                     |
| ------------------------- | ---------------------------------------------------- |
| Flutter / React Native    | Mobile application                                   |
| FastAPI / Node.js         | Backend REST API                                     |
| PostgreSQL + PostGIS      | Shared geospatial report database                    |
| React                     | Future authority dashboard                           |
| Push notification service | Future proximity alerts and notifications            |
| AI / computer vision      | Potential future hazard detection and classification |

## 💻 Run Locally

### Option 1: Open the HTML file

1. Clone or download this repository.
2. Open `index.html` in a modern browser.
3. Keep an internet connection available for Leaflet and OpenStreetMap assets.


## 🌐 Deploy with GitHub Pages

1. Upload `index.html` and `README.md` to the root of your GitHub repository.
2. Commit and push the files to your default branch.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select your default branch and the `/(root)` folder.
6. Click **Save**.
7. Wait for GitHub Pages to publish the site.
8. Open the published URL shown in the Pages settings.


## 📁 Project Structure

```text
road-ai/
├── index.html     # Responsive interactive front-end demo
└── README.md      # Project documentation
```

## 🚀 Future Scope

- Develop a backend API and shared database.
- Add user authentication and authorized reviewer roles.
- Support image uploads and report evidence.
- Improve duplicate detection and report verification.
- Add report freshness indicators and geographic search.
- Integrate with relevant road-authority workflows where partnerships permit.
- Explore AI-based pothole and road-hazard detection using suitable image data.
- Introduce driver-safe proximity alerts and push notifications.
- Build an authority dashboard for prioritization and resolution tracking.
- Test the system in a controlled campus or neighbourhood pilot.

## 🛡 Safety, Privacy, and Limitations

- RoadAI is not an emergency service or an official traffic information source.
- Sample locations and reports are illustrative, not verified live road conditions.
- Do not use or interact with the website while driving. Submit reports only when safely stopped or as a passenger.
- Location access is optional and requires browser permission.
- Demo reports are stored in the current browser and are not shared across users or devices.
- Avoid entering personal or sensitive information.
- The current demo does not perform AI-based hazard detection, independently verify reports, connect to a live road authority, or send real-time alerts.
- The project does not claim measured crash reduction or guaranteed road safety.
- A production release would require backend development, security and privacy review, moderation,
  operational monitoring, and coordination with relevant authorities.

## 👨‍💻 Author

**Vikash Kasaudhan**
B.Tech, 3rd Year
PSIT Kanpur

---

**RoadAI — Know the road before you reach it.**
