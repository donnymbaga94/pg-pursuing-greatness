# P.G — Pursuing Greatness 🚀

> **Transform self-improvement into an immersive RPG. Level up your life,
build ironclad discipline, and track your daily quests.**

---

## 📌 Overview  

**P.G (Pursuing Greatness)** is a gamified goal-tracking and habit-formation platform 
designed to bridge the gap between human intent and consistent daily execution. 
By applying core Role-Playing Game (RPG) mechanics—such as Experience Points (XP), 
Stat Progression, Daily Quests, and Streaks—P.G turns personal development into an 
engaging, quantifiable journey.

Whether training for a marathon, mastering a software stack, or locking down daily 
physical habits, P.G ensures every action contributes directly to your high-level identity.

---

## ✨ Key Features

* 🎮 **Gamified Character Progression**
  * Earn **XP** and level up as you complete tasks.  
  * Allocate points across core stats (**Strength**, **Agility**, **Intellect**, **Discipline**).
* 📜 **Daily Quests & Milestones**
  * Break massive long-term ambitions into manageable **1-day vertical slices**.
  * Dynamic streak counters with "Never Miss Twice" mechanics.
* 📱 **Seamless Cross-Platform Access**
  * **Mobile-First Responsive Web & App UI** tailored for fast, low-friction logging.
  * Instant local state updates with background sync.
* 🔒 **RESTful Architecture**
  * Secure, token-authenticated API endpoints powering both web and mobile frontends.

## 🏗️ Architecture & Tech Stack

P.G utilizes a decoupled architecture where the Django backend operates as a high-performance 
REST API, serving both the web client and future native mobile builds.

```text
  ┌───────────────────────────┐      ┌───────────────────────────┐
  │   Mobile App (Flutter)    │      │    Responsive Web App     │
  └─────────────┬─────────────┘      └─────────────┬─────────────┘
                │                                  │
                └─────────────────┬────────────────┘
                                  │  JSON / REST API
                                  ▼
                     ┌───────────────────────────┐
                     │   Django REST Framework   │
                     │    (Python 3.11+ Core)    │
                     └─────────────┬─────────────┘
                                   │
                                   ▼
                     ┌───────────────────────────┐
                     │  PostgreSQL / SQLite DB   │
                     └───────────────────────────┘
```

# Backend
** Language:       Python 3.11+
** Framework:      Django 5.x
** API Engine:     Django REST Framework (DRF)
** Authentication: Simple JWT/Token Authentication

# Frontend & Mobile
** Mobile & Cross-Platform UI: Flutter/Dart
** Web Client: DJango Templates + Tailwind CSS/HTMX (or SPA integration)

# Project Structure

pg-pursuing-greatness/  
├── config/                 # Project settings & root URL routing  
│   ├── settings.py  
│   ├── urls.py  
│   └── wsgi.py  
├── apps/  
│   ├── users/              # User profiles, level/XP calculations, stats  
│   ├── quests/             # Daily tasks, habits, and milestone tracking  
│   └── gamification/       # Achievements, streak logic, and badges  
├── static/                 # CSS, JavaScript, and asset bundles  
├── templates/              # HTML layout templates  
├── manage.py  
├── requirements.txt  
└── README.md  

# LICENSE

Distributed under the MIT License. See LICENSE for more information

