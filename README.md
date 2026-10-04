# 🚚 TransitOps AI
### Smart Transport Operations Platform

An AI-powered enterprise Transport Operations Management System built to digitize and automate fleet management, dispatch operations, maintenance tracking, fuel monitoring, expense management, and operational analytics.

Built for the **Odoo Hackathon** using **React, TypeScript, Firebase, Tailwind CSS, and AI-powered business automation**.

---

![React](https://img.shields.io/badge/React-19-61DAFB?logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-5.x-3178C6?logo=typescript)
![Firebase](https://img.shields.io/badge/Firebase-Firestore-FFCA28?logo=firebase)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-4.x-38BDF8?logo=tailwindcss)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Hackathon-blue)

---

# 📌 Table of Contents

- Overview
- Business Problem
- Solution
- Key Features
- Workflow
- Business Rules
- Technology Stack
- System Architecture
- Database Design
- Folder Structure
- Installation
- Environment Variables
- Screenshots
- Future Enhancements
- Contributors
- License

---

# 📖 Overview

TransitOps AI is an enterprise-grade Transport Operations Management Platform designed for logistics organizations that still rely on spreadsheets, manual dispatch logs, and disconnected systems.

The platform centralizes vehicle management, driver management, dispatch operations, maintenance tracking, fuel monitoring, expense management, and operational analytics into a single AI-assisted dashboard.

Instead of manually coordinating vehicles, drivers, and maintenance schedules, organizations can automate operational workflows while ensuring compliance with business rules.

---

# 🚨 Business Problem

Many transport companies face challenges such as:

- Manual dispatch planning
- Vehicle scheduling conflicts
- Underutilized fleet
- Missed maintenance schedules
- Expired driver licenses
- Fuel expense mismanagement
- Lack of operational visibility
- Poor business analytics
- Spreadsheet-based tracking
- Human errors during dispatch

These issues increase operational costs while reducing efficiency.

---

# 💡 Solution

TransitOps AI provides a centralized ERP platform that digitizes the complete transport lifecycle.

The system allows organizations to:

- Register vehicles
- Manage drivers
- Dispatch trips
- Track maintenance
- Record fuel logs
- Track operational expenses
- Generate business insights
- Monitor fleet utilization
- Ensure regulatory compliance

The platform also introduces intelligent business automation through AI-assisted operational recommendations.

---

# ✨ Key Features

## 🔐 Authentication

- Firebase Authentication
- Secure Email Login
- Role-Based Access Control
- Protected Routes
- Session Management

---

## 👥 Role-Based Access Control

The platform supports multiple enterprise roles.

### Fleet Manager

Responsible for:

- Vehicle Registry
- Maintenance
- Fleet Health
- Operational Efficiency

---

### Dispatcher

Responsible for:

- Trip Creation
- Driver Assignment
- Vehicle Assignment
- Trip Monitoring

---

### Safety Officer

Responsible for:

- Driver Compliance
- License Validation
- Safety Monitoring
- Driver Risk Tracking

---

### Financial Analyst

Responsible for:

- Fuel Analysis
- Expense Reports
- Vehicle ROI
- Operational Costs

---

# 📊 Dashboard

Enterprise dashboard containing:

- Active Vehicles
- Available Vehicles
- Vehicles in Maintenance
- Active Trips
- Pending Trips
- Drivers On Duty
- Fleet Utilization
- Fuel Consumption
- Operational Cost
- Monthly Analytics

Interactive charts include:

- Fleet Utilization
- Fuel Trend
- Monthly Trips
- Operational Cost
- Vehicle Performance

---

# 🚛 Vehicle Registry

Manage every fleet asset.

Vehicle Information includes:

- Registration Number
- Vehicle Model
- Vehicle Type
- Capacity
- Odometer
- Acquisition Cost
- Vehicle Status

Supported Status

- Available
- On Trip
- In Shop
- Retired

Features

- CRUD
- Search
- Filters
- Sorting
- Pagination
- Status Badges

---

# 👨‍✈️ Driver Management

Maintain driver profiles.

Driver Details

- Name
- License Number
- License Category
- License Expiry
- Contact Number
- Safety Score
- Status

Supported Status

- Available
- On Trip
- Off Duty
- Suspended

Features

- Driver Profiles
- Search
- Filters
- CRUD
- License Expiry Alerts
- Safety Monitoring

---

# 🚚 Trip Management

Create and monitor transport operations.

Trip Information

- Source
- Destination
- Driver
- Vehicle
- Cargo Weight
- Planned Distance
- Trip Status

Trip Lifecycle

Draft

↓

Dispatched

↓

Completed

or

Cancelled

The application automatically updates driver and vehicle status during each stage.

---

# 🔧 Maintenance Management

Manage fleet maintenance operations.

Maintenance Record includes

- Vehicle
- Service Type
- Issue
- Cost
- Service Date
- Maintenance Status

Business Automation

Opening Maintenance

↓

Vehicle automatically becomes

"In Shop"

Closing Maintenance

↓

Vehicle automatically returns to

"Available"

---

# ⛽ Fuel & Expense Management

Track

Fuel Logs

- Fuel Quantity
- Cost
- Mileage
- Date

Expenses

- Toll
- Repair
- Parking
- Insurance
- Miscellaneous

Automatic operational cost calculation.

---

# 📈 Analytics

Business Intelligence Dashboard

Metrics include

- Fuel Efficiency
- Fleet Utilization
- Operational Cost
- Vehicle ROI
- Driver Performance
- Maintenance Cost
- Delivery Statistics

Export

- CSV
- PDF (Optional)

---

# 🤖 AI Features

TransitOps AI introduces intelligent automation.

### AI Route Optimization

Suggests optimal routes based on operational efficiency.

---

### AI Delay Prediction

Predicts delivery delays using

- Distance
- Traffic
- Weather

---

### Predictive Maintenance

Analyzes

- Vehicle Mileage
- Service History

to recommend future maintenance.

---

### Fleet Insights

Provides AI-generated operational recommendations to improve utilization and reduce costs.

---

# ⚙️ Business Rules

The application enforces the following rules.

✔ Registration Number must be unique

✔ Retired vehicles cannot be dispatched

✔ Vehicles under maintenance cannot be dispatched

✔ Suspended drivers cannot be assigned

✔ Expired licenses prevent dispatch

✔ Driver already on a trip cannot be reassigned

✔ Vehicle already on a trip cannot be reassigned

✔ Cargo weight cannot exceed vehicle capacity

✔ Dispatch automatically changes statuses

✔ Completing trips restores availability

✔ Maintenance automatically changes vehicle status

---

# 🔄 Application Workflow

Vehicle Registration

↓

Driver Registration

↓

Trip Creation

↓

Business Validation

↓

Dispatch

↓

Trip Monitoring

↓

Trip Completion

↓

Fuel Logging

↓

Maintenance

↓

Analytics Dashboard

---

# 🏗 Technology Stack

## Frontend

- React
- TypeScript
- TailwindCSS
- Shadcn UI
- Framer Motion
- React Router
- Lucide Icons
- Recharts

---

## Backend

- Firebase Authentication
- Cloud Firestore

---

## Validation

- React Hook Form
- Zod

---

## Deployment

- Firebase Hosting
or
- Vercel

---

# 🗄 Database Collections

```
users
vehicles
drivers
trips
maintenance
fuelLogs
expenses
notifications
```

---

# 📁 Project Structure

```
src/

components/
layouts/
pages/
hooks/
context/
services/
firebase/
routes/
utils/
types/
assets/

```

---

# 🚀 Installation

Clone repository

```bash
git clone https://github.com/yourusername/transitops-ai.git
```

Install dependencies

```bash
npm install
```

Start development server

```bash
npm run dev
```

Build production

```bash
npm run build
```

---

# 🔑 Environment Variables

Create a `.env` file.

```env
VITE_FIREBASE_API_KEY=

VITE_FIREBASE_AUTH_DOMAIN=

VITE_FIREBASE_PROJECT_ID=

VITE_FIREBASE_STORAGE_BUCKET=

VITE_FIREBASE_MESSAGING_SENDER_ID=

VITE_FIREBASE_APP_ID=
```

---

# 🎨 UI Highlights

- Enterprise Dashboard
- Responsive Design
- Glassmorphism Cards
- Beautiful Tables
- Dark Mode
- Animated Sidebar
- Interactive Charts
- Skeleton Loading
- Toast Notifications
- Status Indicators
- Drawer Based Editing
- Mobile Friendly

---

# 📌 Future Enhancements

- Live GPS Tracking
- Google Maps Integration
- AI Chat Assistant
- IoT Vehicle Monitoring
- Driver Mobile App
- Push Notifications
- QR-based Vehicle Inspection
- OCR Document Verification
- Predictive Fuel Optimization
- Multi-company Support

---

# 🤝 Contributors

Developed as part of the **Odoo Hackathon**.

Contributions, issues, and feature requests are welcome.

---

# 📄 License

This project is licensed under the MIT License.

---

<div align="center">

### ⭐ If you found this project useful, don't forget to star the repository!

Made with ❤️ for the Odoo Hackathon

</div>
