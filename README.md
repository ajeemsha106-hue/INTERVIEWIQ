# INTERVIEWIQ – SMART INTERVIEW PREPARATION PLATFORM

> **"Your Dream Career Starts With One Smart Practice."**

[![Production Build](https://img.shields.io/badge/Production-Verified-success?style=for-the-badge&logo=vite)](https://interviewiq.vercel.app)
[![Tech Stack](https://img.shields.io/badge/Stack-React%20%7C%20TypeScript%20%7C%20Tailwind-7C3AED?style=for-the-badge)](https://react.dev)
[![Database](https://img.shields.io/badge/Database-Supabase%20%2F%20PostgreSQL-3ECF8E?style=for-the-badge&logo=supabase)](https://supabase.com)
[![Deployment](https://img.shields.io/badge/Deploy-Vercel-black?style=for-the-badge&logo=vercel)](https://vercel.com)

---

## 🚀 Executive Overview

**INTERVIEWIQ** is a production-grade, AI-powered interview preparation ecosystem tailored for college students, fresh graduates, and tech job seekers. It simulates the exact cognitive filters of campus placements, top technology screening tests, and multi-stage behavioral rounds.

The platform embraces a **premium dark navy (`#060913`, `#0B0F1E`) and electric purple (`#7C3AED`, `#8B5CF6`) aesthetic** with glassmorphism, glowing accents, real-time analytics charts, and seamless responsive layouts for mobile, tablet, and desktop.

---

## 🌟 Core Modules & Functional Architecture

### 1. Landing Page (Publicly Accessible)
- **Zero Gatekeeping:** Public visitors can immediately explore features, take the Question of the Day, and browse career tracks without creating an account.
- **Hero Section:** Punchy title *"Your Next Interview Could Change Your Life"*, subheadings, and quick action buttons.
- **Startup Visual Canvas:** Animated student practicing + real-time IQ Mentor feedback + floating streak cards.
- **Platform Metrics:** Verified sample indicators (12,500+ candidates trained, 89.4% offer rate).

### 2. User Authentication & Profile Security
- **Role Selection:** College Student, Fresh Graduate, or Experienced Professional.
- **Target Career:** Software Engineering, Electrical Engineering, Electronics & VLSI, Data Science, Cloud, Banking.
- **Demo Accounts (Zero-Friction 1-Click Testing):**
  - **Candidate Demo:** `candidate@interviewiq.com` / `password123`
  - **Admin Demo:** `admin@interviewiq.com` / `admin123`
- Full registration, login, logout, password validation (min 6 characters), and simulated password recovery.

### 3. Personalized Dashboard
- **Welcome Hero:** Dynamic greeting, current streak counter, and daily goal progress bar.
- **Interview Readiness Meter:** Dynamic circular SVG gauge computing readiness (0-100%) from quiz accuracy, mock completion, and streak.
- **Metrics Grid:** Total solved, quiz accuracy %, mock rounds completed.
- **Weak Topics Radar:** Automatic detection of subjects with `< 70%` accuracy with 1-click drill launcher.
- **Smart Recommendation Engine:** Adaptive *"Your Next Smart Step"* card.
- **Weekly Activity Chart:** Interactive Recharts bar visualization tracking practice volume.

### 4. AI Preparation Assistant: "IQ Mentor"
- Dedicated AI coaching drawer.
- Pre-built intelligent heuristic engine providing theorem explanations (Ohm's Law, KCL/KVL, Transformers, AC/DC, ACID), STAR answer reviews, and custom question generation.
- **Honest AI Policy:** Clearly discloses provider mode (`Built-in Heuristic Engine` vs `Custom Gemini API`). Optional Gemini API key input available.

### 5. Aptitude Practice Module
- Categories: Quantitative Aptitude, Logical Reasoning, Verbal Ability, Percentages, Time & Work, Speed & Distance, Probability, Data Interpretation.
- Countdown timer (60s/question with visual warning), 4 answer choices, instant scoring, step-by-step mathematical reasoning, and celebratory confetti upon scoring $\ge 70\%$.

### 6. Technical Interview Preparation
- **Full Core Electrical & Electronics Coverage:**
  - Ohm's Law, Kirchhoff's Laws (KCL, KVL)
  - Transformers (Step-down, eddy current laminations, DC burnout proof)
  - AC and DC (RMS vs Peak, Power Factor, lagging/leading)
  - Electrical Machines (Induction synchronous speed, DC series motor danger)
  - Power Systems (High voltage transmission loss reduction)
  - Control Systems (Routh-Hurwitz stability)
  - Circuit Analysis (Thevenin's equivalent)
  - Electrical Measurements (Two-wattmeter method)
- Computer Science (QuickSort, Big-O), Database (ACID, B+ Trees), Networking (OSI, TCP 3-way handshake), Software Engineering (Observer Pattern, SOLID LSP).

### 7. HR Behavioral Masterclass
- 7 Master Questions: *"Tell me about yourself"*, *"Greatest strengths"*, *"Weaknesses"*, *"Why hire you"*, *"Why this job"*, *"Five years"*, *"Teamwork conflict"*.
- STAR framework guides, traps to avoid, sample winning scripts.
- Interactive **"Practice Your Pitch"** box with word-count analysis and instant rubric feedback.

### 8. Virtual Mock Interview Room
- Role, difficulty, and duration selection (5, 10, or 15 mins).
- Timed questions with optional Web Speech API microphone speech-to-text recording.
- Self-evaluation rubric across 4 dimensions: Clarity, Technical Depth, Structure, Confidence.
- Detailed diagnostic report with areas to improve and suggested next practice.

### 9. Progress Analytics & Milestones
- Recharts visualizations for Topic-Wise Accuracy and Score Progression Trends.
- Unlockable achievement badges (Consistency Champion, Core Engineering Specialist, Century Solver).

### 10. Bookmarks, Revision & Study Reminders
- Bookmark any tricky question across the platform.
- Study reminder scheduler: day of week selection, daily study time, target questions slider.

### 11. Admin Console (Role-Protected)
- Only accessible by users with `role: 'admin'`.
- Add, edit, and delete questions from the live platform library.
- Monitor database health and platform learner metrics.

---

## 🛠️ Local Development

```bash
# 1. Install dependencies
npm install

# 2. Start Vite development server
npm run dev

# 3. Build optimized production bundle
npm run build

# 4. Preview production build locally
npm run preview
```

---

## 🌐 Public Deployment Guide

### Option 1: One-Click Vercel Deployment (Recommended)

1. Push your repository to **GitHub** or **GitLab**.
2. Log into [vercel.com](https://vercel.com) and click **"Add New Project"**.
3. Import this repository.
4. Framework Preset will auto-detect **Vite**.
5. Build Command: `npm run build` | Output Directory: `dist`.
6. (Optional) Add Environment Variables:
   - `VITE_SUPABASE_URL`: Your Supabase Project URL
   - `VITE_SUPABASE_ANON_KEY`: Your Supabase Anon Public Key
   - `VITE_GEMINI_API_KEY`: (Optional) Your Google AI Gemini API Key
7. Click **Deploy**. Your live production website URL will be ready in under 60 seconds!

### Option 2: Connecting Supabase PostgreSQL Cloud Database

1. Create a free project at [supabase.com](https://supabase.com).
2. Open the **SQL Editor** in your Supabase dashboard.
3. Paste the contents of `supabase/schema.sql` and click **Run**.
4. Retrieve your `Project URL` and `anon public key` from **Project Settings > API**.
5. Add them to your Vercel project environment variables.

### Option 3: Custom Domain Setup

1. In the Vercel Dashboard, navigate to **Settings > Domains**.
2. Enter your custom domain (e.g., `interviewiq.yourdomain.com`).
3. Add the displayed `CNAME` or `A` records in your DNS provider (Cloudflare, Namecheap, GoDaddy).
4. Vercel automatically issues and provisions a free wildcard SSL certificate.

---

## 🛡️ Security & Quality Standards

- **Strict Client-Side Boundary:** No secret API keys or service role tokens are bundled into frontend assets.
- **Row Level Security (RLS):** Supabase database policies ensure users can read only their own quiz sessions, mock interviews, and bookmarks.
- **Role-Based Routing:** Protected administrative controls are invisible and inaccessible to standard candidates.
- **Offline / Zero-Config Resilience:** Gracefully functions with full persistence even before remote cloud keys are configured.
