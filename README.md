# FuelTracker

A smart tracker for your vehicle's fuel fill-ups, maintenance history, and running costs. Use it to track your true fuel mileage and get automatic alerts before scheduled service is due.

***Live Site:*** [https://fueltracker-app.pages.dev](https://fueltracker-app.pages.dev)

---

> ### ⚠️ Project Disclaimer
> **This is strictly a non-commercial, educational hobby project.** 
> **All application architecture, user interface design, logic, and source code in this repository were completely generated using Artificial Intelligence (AI).** It is maintained solely for learning, personal experimentation, and prototyping purposes.

---

## Overview
Vehicle Fuel and Maintenance Tracker is a responsive web application designed for motorists to log refueling entries, monitor vehicle fuel efficiency, track maintenance history, and receive timely service interval alerts. Built with an offline-first architecture, the application stores data locally via localStorage while offering real-time cloud synchronization through Firebase Authentication and Cloud Firestore.

## Tech Stack
- Frontend: HTML5, JavaScript (ES6+), TypeScript
- Styling: Tailwind CSS
- Data Visualization: Chart.js
- Iconography: Lucide Icons
- Cloud and Backend: Firebase Authentication, Cloud Firestore
- PWA Support: Service Worker, Web App Manifest
- Bundler and Tooling: Vite

## Features
- Refueling Management: Record fill-up date, current odometer reading, fuel volume in liters, and total cost. Inline edit and delete capabilities allow quick adjustments.
- Real-Time Fuel Analytics: Automatically computes overall average fuel efficiency (km/L), latest trip mileage, total kilometers tracked, and cumulative fuel expenditure.
- Interactive Analytics Charts: Chart.js visualizations display mileage trends and per-liter fuel cost fluctuations over time with filtering options (3 months, 6 months, 12 months, or all time).
- Maintenance Log: Maintain service records by category (e.g., General Service, Engine Oil Change, Tires/Wheels, Brakes, Battery) with associated costs and notes.
- Service Interval Alerts: Dynamically monitors distance driven since the last maintenance event and warns the user when the vehicle is within 500 km of a scheduled service interval.
- Data Portability: Export and restore records using standard CSV format. Includes an unstructured text parser to quickly paste and import batch records.
- User Authentication and Cloud Sync: Secure email/password login syncs logs to Firebase Cloud Firestore for multi-device access with automatic offline fallback.
- Responsive UI and Dark Mode: Adapts across mobile, tablet, and desktop screens with toggleable light and dark themes.
