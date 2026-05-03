# 💊 MediCare — Medicine Reminder

A premium dark-themed mobile app UI prototype for medicine reminders, built as a pair of companion apps — one for the **elder** and one for their **caretaker**.


---

## 📱 Apps

### 1. MediCare — Elder App (`medireminder.html`)
The patient-facing interface. Designed for elderly users with a warm copper-toned dark theme for comfort and readability.

**Screens:**
- **Splash** — Animated welcome screen with app branding
- **Home** — Today's medicine schedule with Taken / Due / Upcoming badges
- **All Medicines** — Full list of prescribed medications
- **Medicine Detail** — Dosage info, timeline, and intake history
- **Add Medicine** — Form to add a new medicine with schedule
- **Reminder Alert** — Full-screen alert for due medicines
- **Profile** — User profile with caregiver contact strip
- **Widgets** — Quick-access widget previews

---

### 2. CareView — Caretaker App (`medicare_caretaker.html`)
The caretaker-facing companion interface. Steel-blue dark theme to visually differentiate roles.

**Screens:**
- **Splash** — "Stay in touch with every dose, every day" — role-identified entry screen
- **Dashboard** — Patient adherence ring (%), taken/pending/missed stats, missed dose alerts, today's full schedule, quick actions
- **Patient Progress** — Per-medicine course tracking (Day X of Y), progress bars, 7-day color-coded adherence dots
- **Add Medicine** — Caretaker-specific form: Prescribed By, Course Duration, private Caretaker Note, "Alert me if missed" toggle — saves & syncs to elder app
- **Activity Log & Notes** — Chronological event timeline (Today / Yesterday / This Week), inline "Mark as Taken", note modal with quick tags (#Dose late, #Side effect, #Doctor call, #Good day)
- **Profile & Settings** — Adherence stats, linked patient section, notification toggles, Export Progress Report

---

## 🗂️ Project Structure

medireminder/
├── medireminder.html         # Elder-facing MediCare app
├── medicare_caretaker.html   # Caretaker-facing CareView app
└── README.md

---

## 🎨 Design System

| Property | Elder App | Caretaker App |
|---|---|---|
| Primary Accent | Copper `#B5602A` | Steel Blue `#3A80D2` |
| Background | `#0E0B0F` | `#090B0E` |
| Surface | `#1A1118` | `#111620` |
| Font (Headings) | Playfair Display | Playfair Display |
| Font (Body) | Lato | Lato |
| Frame | 375 × 812 px | 375 × 812 px |

**Shared design tokens:** `--green` (taken), `--crimson` (missed), `--amber` (overdue), `--parchment` (primary text)

---

## 🚀 How to Run

No build step, no dependencies, no server required.

1. Clone or download the repo
2. Open either HTML file directly in a browser:
open medireminder.html
open medicare_caretaker.html

3. Navigate between screens using the bottom navigation bar and interactive buttons

---

## 🔧 Tech Stack

- **HTML5** — Single-file SPA per app
- **CSS3** — Custom properties, Flexbox, CSS animations (`@keyframes`)
- **Vanilla JavaScript** — Screen routing via `go(screenId)`, modal overlays
- **Google Fonts** — Playfair Display + Lato
- **SVG** — Inline icons, circular progress rings (`stroke-dasharray`)
- **No frameworks. No dependencies. No build tools.**

---

## ✨ Key Features

- 📱 Realistic phone shell mockup (notch, rounded corners, status bar)
- 🌑 Premium dark theme — no eye strain for elderly users
- 🔄 Sync flow — medicines added by caretaker reflect on elder's app
- 📊 Course duration tracking — Day X of Y with progress bar
- 🟢 7-day adherence dots — color-coded intake history per medicine
- 📝 Caretaker notes — private observations with quick tags
- 🔔 Missed dose alerts — banner and full-screen reminder
- 📤 Export progress report option (UI only)

---

## 👥 Roles

| Role | App | Purpose |
|---|---|---|
| Elder / Patient | `medireminder.html` | View schedule, mark doses taken, receive reminders |
| Caretaker / Family | `medicare_caretaker.html` | Monitor adherence, add medicines, log observations |

---
