<div align="center">

# 🏥 MediCare HMS
### A Modern, Role-Based Hospital Management System

Streamlining hospital operations — from patient registration to discharge — through dedicated, role-specific dashboards.

[![React](https://img.shields.io/badge/React-19-61DAFB?logo=react&logoColor=white)](https://react.dev/)
[![Vite](https://img.shields.io/badge/Vite-8-646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)
[![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-4-06B6D4?logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![React Router](https://img.shields.io/badge/React_Router-7-CA4245?logo=reactrouter&logoColor=white)](https://reactrouter.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)

[**Live Demo**](#) &nbsp;•&nbsp; [Features](#-features) &nbsp;•&nbsp; [Tech Stack](#-tech-stack) &nbsp;•&nbsp; [Getting Started](#-getting-started) &nbsp;•&nbsp; [Roadmap](#-roadmap)

</div>

---

## 📋 Overview

**MediCare HMS** is a full-featured Hospital Management System frontend built to handle the day-to-day workflow of a hospital across **7 distinct roles** — Admin, Doctor, Nurse, Receptionist, Lab Technician, Pharmacist, and IP (In-Patient) Manager. Each role gets its own dashboard, navigation, and permissions, so every user sees only what's relevant to their job — from patient check-in to lab results to prescription dispensing.

> 🚧 The project currently runs on an in-memory data store with role-based mock authentication, with a real Node/Express/MongoDB backend planned next. See [Roadmap](#-roadmap).

## ✨ Features

| Role | What they can do |
|---|---|
| 🧑‍💼 **Admin** | Manage doctors & staff, finance overview, vehicle/ambulance records, reports, follow-ups |
| 👨‍⚕️ **Doctor** | Patient consultation, diagnosis, prescriptions, lab & radiology orders, follow-up management |
| 💉 **Nurse** | Patient queue, vitals entry & history tracking |
| 🛎️ **Receptionist** | Patient registration, appointment scheduling, queue management, billing & collections |
| 🧪 **Lab Technician** | Test orders, sample collection, result entry, report management |
| 💊 **Pharmacist** | Medicine inventory, prescription queue, dispensing, billing |
| 🛏️ **IP Manager** | Admissions, bed management, current in-patients, discharge processing, reports |

**Core platform features:**
- 🔐 Role-based authentication with protected routes
- 📊 Reusable dashboard components — stats cards, data tables, status badges
- 🎨 Clean, responsive UI built with Tailwind CSS
- 🧭 Dedicated sidebar & navigation per role
- ⚡ Fast dev experience powered by Vite

## 🛠️ Tech Stack

**Frontend**
- [React 19](https://react.dev/) — UI library
- [Vite](https://vitejs.dev/) — build tool & dev server
- [Tailwind CSS 4](https://tailwindcss.com/) — styling
- [React Router 7](https://reactrouter.com/) — client-side routing
- [Axios](https://axios-http.com/) — HTTP client (wired up for the upcoming backend)

**Planned Backend** *(see [Roadmap](#-roadmap))*
- Node.js + Express
- MongoDB
- JWT-based authentication

## 📸 Screenshots

<div align="center">
<i>Add screenshots or a demo GIF of the Login page and a couple of role dashboards here.</i>
</div>

## 🚀 Live Demo

🔗 **[View Live Site](#)** *(add your deployed link here once live)*

**Demo logins** (role-based, no password required in the current mock-auth build):

| Role | Login as |
|---|---|
| Doctor | `doctor` |
| Receptionist | `receptionist` |
| Nurse | `nurse` |
| Pharmacist | `pharmacy` |
| Lab Technician | `lab` |
| IP Manager | `ipmanager` |
| Admin | `admin` |

## 🏁 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) v18 or higher
- npm

### Installation

```bash
# Clone the repository
git clone https://github.com/MD-NABEEL-T/HMS.git
cd HMS

# Install dependencies
npm install

# Start the development server
npm run dev
```

The app will be running at `http://localhost:5173`.

### Build for production

```bash
npm run build
npm run preview
```

## 📁 Project Structure

```
src/
├── components/
│   └── common/         # Shared components (Sidebar, Header, StatsCard, DataTable, StatusBadge)
├── context/
│   └── AuthContext.jsx # Role-based auth state
├── pages/
│   ├── admin/
│   ├── doctor/
│   ├── nurse/
│   ├── receptionist/
│   ├── lab/
│   ├── pharmacy/
│   ├── ip/
│   └── auth/
├── routes/
│   └── ProtectedRoute.jsx
├── services/
│   └── api.js           # Axios instance for backend calls
└── store/
    └── hospitalStore.jsx # Centralized app state (seed/mock data)
```

## 🗺️ Roadmap

- [ ] Node/Express/MongoDB backend with real data persistence
- [ ] JWT-based authentication (replacing mock login)
- [ ] Real-time notifications (appointments, lab results, bed availability)
- [ ] Role-based access control enforced server-side
- [ ] Deployment of full-stack app (frontend + backend + database)

## 🤝 Contributing

This project was built collaboratively, with each module owned by a different contributor. Contributions, issues, and feature requests are welcome — feel free to check the [issues page](https://github.com/MD-NABEEL-T/HMS/issues).

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## 👤 Author

**Mohammed Nabeel T**

- GitHub: [@mdnabeelt](https://github.com/mdnabeelt) / [@MD-NABEEL-T](https://github.com/MD-NABEEL-T)

---

<div align="center">

If you found this project useful, consider giving it a ⭐!

</div>
