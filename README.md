<!-- ================================================= -->
<!--                INTERN HUB README                  -->
<!-- ================================================= -->

<div align="center">

# 🚀 Intern Hub  
### The Internship Operating System

<p>
  <img src="https://img.shields.io/badge/Next.js-14+-000000?style=for-the-badge&logo=nextdotjs" />
  <img src="https://img.shields.io/badge/TailwindCSS-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white" />
  <img src="https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/Framer%20Motion-black?style=for-the-badge&logo=framer" />
</p>

**A full-stack internship workflow platform for ambitious students and performance-driven recruiters.**

From application → review → shortlist → hire.  
Everything centralized. Everything tracked.

</div>

---

# 🌍 Problem It Solves

Internship workflows are fragmented.

Students:
- Apply blindly  
- Track nothing  
- Repeat data entry  

Recruiters:
- Use spreadsheets  
- Manually track applicants  
- Lose visibility  

Intern Hub replaces chaos with structured workflow.

---

# ✨ Features

## 🎓 For Students

- 📍 Real-time application status timeline  
- 🗂 Central dashboard for all active roles  
- ⚡ One-click apply using saved profile  
- 📄 Clean internship detail pages  
- 🔎 Filter applications by status  

---

## 💼 For Recruiters

- 📊 Real-time applicant counter  
- 🏷 Tag-based skill input system  
- 🔄 Activate / Suspend listings  
- 👥 Candidate status control (Shortlist / Hire / Reject)  
- 📂 Centralized listing management  

---

# 🧠 Architecture Overview

<details>
<summary><strong>System Flow Diagram</strong></summary>

```
Client (Next.js 14 App Router)
        ↓
Supabase Auth (JWT)
        ↓
PostgreSQL (Relational Schema + TEXT[] arrays)
        ↓
Real-Time Subscriptions
```

</details>

---

# 🛠 Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | Next.js 14 (App Router) |
| Styling | Tailwind CSS |
| Backend | Supabase |
| Database | PostgreSQL |
| Authentication | Supabase Auth |
| Animations | Framer Motion |
| Icons | Lucide React |

---

# 🗄 Database Structure

<details>
<summary><strong>Core Tables</strong></summary>

### `users`
Role-based identity management (student / recruiter)

### `student_profiles`
Resume URL, skill data, linked to users

### `recruiter_profiles`
Company metadata

### `internships`
Role details + TEXT[] skill tags + active status

### `applications`
Student ↔ Internship relationship  
Unique constraint prevents duplicate applications

### `community_posts`
Shared announcements

</details>

---

# 🚦 Getting Started

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/yashwanth-maram/intern-hub1.git
cd intern-hub1
```

---

## 2️⃣ Install Dependencies

```bash
cd app
npm install
```

---

## 3️⃣ Environment Setup

Create `.env.local` inside `/app`

```env
NEXT_PUBLIC_SUPABASE_URL=your_project_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_anon_key
```

---

## 4️⃣ Start Development Server

```bash
npm run dev
```

Visit:  
`http://localhost:3000`

---

# 🎨 Design Philosophy

- High-contrast premium UI  
- Deep charcoal core (#383838)  
- Rounded geometry (`rounded-[40px]`)  
- Glassmorphism components  
- Micro-interactions via Framer Motion  
- Accessibility-first typography  

Minimal noise. Maximum clarity.

---

# 📸 UI Preview (Replace With Real Screenshots)

```
Add your screenshots here:

/assets/student-dashboard.png
/assets/recruiter-dashboard.png
/assets/internship-detail.png
```

Example embed:

```markdown
![Dashboard Preview](assets/student-dashboard.png)
```

---

# 📈 Future Roadmap

- 🤖 AI-based internship recommendations  
- 📊 Recruiter analytics dashboard  
- 📬 Email + notification automation  
- 🧠 Resume parsing with embeddings  
- 🔍 Intelligent skill matching  

---

# 🤝 Contributing

```bash
git checkout -b feature/amazing-feature
git commit -m "feat: add amazing feature"
git push origin feature/amazing-feature
```

Open a Pull Request.

---

# 📜 License

Distributed under the MIT License.

---

<div align="center">

### ⭐ If you find this project useful, consider giving it a star.

Intern Hub — Internship Infrastructure Reimagined.

</div>
