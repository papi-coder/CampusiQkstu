# ⬡ CampusIQ — Kumasi Technical University
### Powered by Papi

---

## 📁 Project Structure

```
campusiq/
├── frontend/
│   ├── index.html       ← Main app (Student / Lecturer / HOD login)
│   └── courses.html     ← Course Catalogue + My Courses + Campus Locator
├── backend/
│   └── admin.html       ← Backend Admin Dashboard
└── README.md
```

---

## 🔐 Login System

All accounts are created by the admin only — no hardcoded passwords.

### Admin Login (backend/admin.html)
| Username | Password  |
|----------|-----------|
| admin    | admin123  |
> Change password in Settings after first login.

### Student / Lecturer / HOD Login (frontend/index.html)
- Accounts created by admin in the backend
- Login with email + password the admin set
- No account = cannot log in

---

## 🚀 Quick Setup

1. Open `backend/admin.html` → login as `admin / admin123`
2. Click **Add Student** → fill name, email, password, ID, programme
3. Credentials shown on screen — copy and share with the student
4. Student opens `frontend/index.html` → selects role → enters email + password → in!

---

## 📚 New Features

### Course Catalogue (courses.html)
- **11 detailed courses** across Applied Sciences, Engineering, Business, Arts
- Full **course descriptions**, learning outcomes, assessments
- **Weekly syllabus** breakdown for every course
- **Prerequisites** shown — checks if you've already enrolled in required courses
- **Resource downloads** — click Download to save course outlines, notes, past questions
- **Enrol** in any course → tracked in My Courses
- **★ Mark as Interested** — save courses you want to take later
- **Filter** by faculty, enrolled, interested, or search by name/code/lecturer

### My Courses Dashboard (courses.html → My Courses tab)
- Live stats: enrolled count, credits, interested count, progress %
- **Animated progress ring** showing semester completion
- **Upcoming deadlines** per enrolled course
- **Unenrol** from any course with one click
- Quick enrol from the interested list

### Campus Student Locator (courses.html → Campus Locator tab)
- **Full privacy controls panel** — every toggle explained
  - Share My Location (on/off)
  - Show My Name (others see your name or just a dot)
  - Show Exact Location (off = building-level only)
  - Discoverable by Friends Only
- **Live campus SVG map** with animated student dots
- **Busy areas panel** — see which buildings are crowded
- **Online students list** — who's currently sharing
- Click any student dot to see their name + programme
- Stop sharing instantly with ✕ Stop button
- Privacy-first: no data stored, live only while active

---

## 🤖 Papi AI — Always Works

Papi AI uses the built-in Claude API (no key needed in Claude.ai artifacts).
When hosted on Netlify or your own server, Papi uses a smart offline fallback
covering Big O, calculus, GPA tips, careers, machine learning, Python, and more —
so students always get a helpful answer even without an API connection.

---

## 💻 View in VS Code

1. Extract the zip → open `campusiq` folder in VS Code
2. Install **Live Server** extension (Ritwick Dey)
3. Right-click `frontend/index.html` → **Open with Live Server**
4. Right-click `frontend/courses.html` → **Open with Live Server** (separate tab)
5. Right-click `backend/admin.html` → **Open with Live Server**

---

## 🌐 Host Free on Netlify

1. Go to **netlify.com** → sign up free
2. **Add new site** → **Deploy manually**
3. Drag the entire `campusiq` folder
4. Live instantly at e.g. `campusiq-kstu.netlify.app`
5. Access:
   - Student app: `/frontend/index.html`
   - Course catalogue: `/frontend/courses.html`
   - Admin backend: `/backend/admin.html`

---

## ✨ Features Summary

### frontend/index.html
- Role login: Student, Lecturer, HOD (admin-created accounts only)
- Student Dashboard: GPA ring, tasks, AI insight, quick actions
- Papi AI Tutor: full Claude AI + smart offline fallback (always answers)
- Smart Schedule with day selector
- Career IQ with internship matching
- Social feed & events

### frontend/courses.html
- 11 KsTU courses with full details
- Syllabus download (saves as .txt)
- Prerequisites checker
- Enrol / Unenrol / Mark as Interested
- My Courses progress dashboard
- Campus Live Locator with full privacy controls

### backend/admin.html
- Create Student, Lecturer, HOD accounts
- View/Delete any account
- Credentials shown after creation with Copy buttons
- All accounts stored in browser localStorage
- Exams, Results, Timetable, Fees, Hostels management
- Papi AI config panel + system logs

---

Built with ❤️ for KsTU · Powered by Papi
