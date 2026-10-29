<div align="center">

# 🎓 College Connect — A Verified Campus Communication Platform

**A secure, college-exclusive platform that centralizes announcements, helps freshers connect with seniors, and uses Gemini AI to make academic communication clearer.**

[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen?style=for-the-badge&logo=vercel)](https://my-hackathon-mvp-of-gdg.vercel.app/)
[![Demo Video](https://img.shields.io/badge/Demo-Video-red?style=for-the-badge&logo=googledrive)](https://drive.google.com/drive/folders/1PDgYueGxes2h6j0VnvNa8V3ycJqVJBZb?usp=drive_link)
![React](https://img.shields.io/badge/React-Vite-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Firebase](https://img.shields.io/badge/Firebase-Auth%20%7C%20Firestore-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![Gemini](https://img.shields.io/badge/Google-Gemini%20AI-4285F4?style=for-the-badge&logo=googlegemini&logoColor=white)

**Google Developer Group on Campus (GGV) · HackXSprint · Problem Statement: Open Innovation**

</div>

---

## 📌 Team Details

| | |
|---|---|
| **Team Name** | Quantum Coders |
| **Team Leader** | Mandakni |
| **Hackathon** | HackXSprint — GDG On Campus, GGV |
| **Problem Statement** | Open Innovation |

---

## 📖 Table of Contents

- [Problem Statement](#-the-problem)
- [Our Solution](#-our-solution)
- [Key Features](#-key-features)
- [Innovation & Opportunities](#-innovation--opportunities)
- [Google Technologies Used](#-google-technologies-used)
- [Architecture](#-architecture)
- [Tech Stack](#-tech-stack)
- [Getting Started](#-getting-started)
- [Future Roadmap](#-future-roadmap)
- [Important Links](#-important-links)
- [Team](#-team)

---

## ❗ The Problem

Colleges rely on scattered, informal channels for official communication. This causes real problems for students:

| Problem | Impact |
|---|---|
| **Open social platforms** allow outsiders | Privacy risks and unsafe student interactions |
| **Freshers have no single reliable source** of information | Difficulty finding guidance and connecting with seniors |
| **Manual verification** is slow and error-prone | Hard to scale |
| **Announcements get buried in casual chats** | Missed deadlines and confusion |
| **Lengthy, poorly written notices** | Reduced understanding among students |
| **No department/year-based organization** | Students receive irrelevant information |

---

## 💡 Our Solution

A **centralized, college-exclusive platform** where only verified students can access official announcements, discussions, and one-to-one interaction — enhanced with **Gemini AI** to rewrite, summarize, and explain content.

- 🔒 **Secure authentication** restricts access to verified college students only.
- 🏫 **Centralized platform** for guidance, announcements, and senior–fresher interaction.
- 🏷️ **Department & academic-year tagging** delivers targeted communication to the right groups.
- 📰 **Structured announcement feed** keeps important updates visible and organized.
- 🤖 **Gemini AI tools** rewrite, summarize, and explain content clearly.
- ✅ **Admin verification** today, with **AI-powered automatic verification** planned.

---

## ✨ Key Features

### 🔐 Secure Access & Account Control
- Email-based signup and login
- Session-based authentication with persistent auth state
- Verified user-only platform entry
- Account-level permission enforcement
- Secure logout and session handling

### 👤 Student Profile System
- Dedicated student profiles with profile image support
- Department and academic-year tagging
- Verified identity display
- Controlled profile updates and secure profile data storage

### 📰 Structured Content Management
- Centralized announcement feed
- Department-filtered content visibility
- Chronological post ordering
- Comment-based interaction on posts

### ✍️ Post Creation & Interaction
- Rich text post creation
- Edit and update your own posts
- Like and comment functionality
- Timestamped content tracking

### 💬 Real-Time Messaging
- One-to-one private messaging
- Real-time delivery with persistent chat history
- Secure, participant-only conversations

### 🧭 Navigation & Dashboard
- Unified student dashboard
- Quick access to recent activity
- Clean, intuitive layout with a minimal learning curve

### ⚙️ Performance & Reliability
- Real-time updates without page refresh
- Optimized frontend and efficient database queries
- Low-latency data fetching

### 🛠️ Admin-Oriented Controls
- Admin-only access to verification tools
- User status management
- Extendable admin dashboard and scalable moderation design

---

## 🚀 Innovation & Opportunities

| # | Highlight | Description |
|---|---|---|
| 1 | **College-Exclusive Verified Platform** | Students upload a valid college ID during signup — unlike public social media, there is real identity validation. |
| 2 | **Digitizing Official Communication** | Replaces informal chat groups with a secure, centralized system for announcements, discussions, and interaction. |
| 3 | **Fresher–Senior Interaction** | Freshers can easily reach out to seniors for guidance, helping to reduce ragging-related problems. |
| 4 | **AI-Enhanced Communication** | Gemini AI rewrites, summarizes, and explains posts without changing the original intent. |
| 5 | **One-to-One Interactive Platform** | Find registered students (filter by year and department) and chat without exposing phone numbers — only name, year, department, and email are shown. |
| 6 | **News Dashboard for College** | An admin-managed dashboard for all official activities, solving delayed or missing updates. |
| 7 | **Centralized Clubs Community** | Tech and extracurricular clubs share activities, promote themselves, and gather audiences for events in one place. |
| 8 | **Improved Student Engagement** | Structured feeds, real-time chat, and AI assistance make communication more interactive and accessible. |
| 9 | **Scalable Campus-Wide Adoption** | Can be adopted across departments, campuses, and institutions with institution-specific rules. |
| 10 | **Future AI-Based Verification** | Gemini AI will analyze email domains and ID documents for fully automated onboarding. |

---

## 🔧 Google Technologies Used

| Technology | Role in the Project |
|---|---|
| **Firebase Authentication** | Secure email-based signup/login; manages sessions and auth state; supports role-based access (student vs. admin). |
| **Firebase Security Rules** | Allows only authenticated users to read/write protected collections; users can modify only their own profiles, posts, and messages; chats are restricted to participants; provides server-side enforcement. |
| **Cloud Firestore** | Scalable NoSQL database for users, posts, comments, and messages; real-time sync for feeds, chats, and dashboards; flexible querying for department-wise retrieval. |
| **Gemini AI (API Key)** | Rewrites posts professionally, summarizes long announcements, explains complex information, powers conversational AI, and will enable automatic ID verification. |

**Additional benefits:** Offline & hybrid support · Future-proof & upgradable · Cost-effective & scalable

---

## 🏗️ Architecture

```
┌──────────────┐      ┌─────────────────────────────┐      ┌──────────────────────┐
│   Frontend   │      │    Firebase Cloud Platform  │      │   Intelligence Layer │
│              │      │                             │      │                      │
│ React +      │ ───► │  Firebase Authentication    │ ───► │  Google Gemini AI    │
│ Tailwind CSS │      │  Cloud Firestore (real-time)│      │  ├─ AI Summarization │
│ (Vite)       │ ◄─── │  Users · Posts · Messages   │ ◄─── │  └─ AI Chat Bot      │
└──────────────┘      └─────────────────────────────┘      └──────────────────────┘
       ▲
       │
  User (Student / Admin)
```

> 📎 *Add the architecture diagram, process flow, and use-case diagram images from the presentation to a `/docs` or `/assets` folder and reference them here:*
>
> `![Architecture Diagram](./assets/architecture.png)`

---

## 🧰 Tech Stack

| Layer | Technology |
|---|---|
| **Frontend** | React, Tailwind CSS, Vite |
| **Authentication** | Firebase Authentication |
| **Database** | Cloud Firestore (real-time) |
| **Security** | Firebase Security Rules |
| **AI** | Google Gemini API |
| **Deployment** | Vercel |

---

## 🏁 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) v18 or higher
- A [Firebase](https://console.firebase.google.com/) project (Authentication + Firestore enabled)
- A [Gemini API key](https://aistudio.google.com/app/apikey)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/Pratyush25ranjan/My-Hackathon-MVP-of-GDG.git

# 2. Move into the project directory
cd My-Hackathon-MVP-of-GDG

# 3. Install dependencies
npm install
```

### Environment Variables

Create a `.env` file in the project root:

```env
VITE_FIREBASE_API_KEY=your_firebase_api_key
VITE_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
VITE_FIREBASE_PROJECT_ID=your_project_id
VITE_FIREBASE_STORAGE_BUCKET=your_project.appspot.com
VITE_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
VITE_FIREBASE_APP_ID=your_app_id
VITE_GEMINI_API_KEY=your_gemini_api_key
```

> ⚠️ Never commit your `.env` file. Make sure it is listed in `.gitignore`.

### Run Locally

```bash
npm run dev
```

The app will be available at `http://localhost:5173`.

### Build for Production

```bash
npm run build
```

---

## 🔮 Future Roadmap

- [ ] 🤖 **AI-Based Automatic Verification** — Gemini AI reads uploaded student ID documents for instant identity confirmation and cross-validates data to detect fake or suspicious accounts.
- [ ] 📱 **Mobile App (Android / iOS)** — On-the-go access, push notifications, and a native smartphone experience.
- [ ] 💬 **Group Chats** — Department-wise, class-wise, or club-based group communication.
- [ ] 🔔 **Notification System** — Real-time alerts for announcements and messages, with priority notifications for urgent academic notices.
- [ ] 📚 **Material Hub (Notes & PYQs)** — A centralized repository for professor notes and previous-year questions.
- [ ] 🔮 **Feedback, Complaint Box & Lost and Found** — Secure feedback submission and an AI-categorized lost-items feed that can be cross-referenced with locations or departments.

---

## 🔗 Important Links

| Resource | Link |
|---|---|
| 💻 **GitHub Repository** | [Pratyush25ranjan/My-Hackathon-MVP-of-GDG](https://github.com/Pratyush25ranjan/My-Hackathon-MVP-of-GDG) |
| 🧪 **Live MVP** | [my-hackathon-mvp-of-gdg.vercel.app](https://my-hackathon-mvp-of-gdg.vercel.app/) |
| 🎥 **Demo Video & Snapshots** | [Google Drive Folder](https://drive.google.com/drive/folders/1PDgYueGxes2h6j0VnvNa8V3ycJqVJBZb?usp=drive_link) |

---

## 👥 Team

**Team Quantum Coders** — Team Leader: **Mandakni**

*Add teammates here:*

| Name | Role | GitHub |
|---|---|---|
| Mandakni | Team Leader | [@username](https://github.com/username) |
| | | |

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open an [issue](https://github.com/Pratyush25ranjan/My-Hackathon-MVP-of-GDG/issues) or submit a pull request.

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<div align="center">

Built with ❤️ by **Team Quantum Coders** for **HackXSprint** · Google Developer Group On Campus, GGV

⭐ *If you like this project, give it a star!*

</div>
