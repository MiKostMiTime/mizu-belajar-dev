# 🚀 Mizu Belajar Dev — Revised Roadmap 2026

> **Roadmap 5 tahun untuk menjadi engineer yang tidak bisa digantikan AI.**
> Direvisi khusus untuk mahasiswa OSN Informatika dengan target masuk CS university dan membangun portfolio yang compelling.

---

## 🎯 Executive Summary

| Timeline | Fokus Utama | Key Outcome |
|----------|-------------|-------------|
| **Year 1** | Full-Stack Web + Mobile (iOS + Android) + AI Fundamentals | 15+ projects, 3-4 capstones, publishable apps |
| **Year 2** | Depth in specialization + Real-world experience | Freelance/internship, income first |
| **Year 3** | Professional engineering + System design | Team collaboration, production scale |
| **Year 4** | Leadership + Architecture + Emerging tech | Tech decisions, mentoring |
| **Year 5** | Unreplaceable engineer + Multiple income streams | CTO/lead/senior IC trajectory |

### 왜 (Mengapa) Saya Revisi:

```
ORIGINAL:
├── iOS only (kurang Android)
├── AI terasa como tambahan, bukan integrated
├── Fase 4 (Backend) terasa repetitive dengan OSN fundamentals
└── Project suggestions kurang "eye-catching" untuk admissions

REVISED:
├── Mobile: iOS + Android (Flutter/React Native)
├── AI: Integrated di setiap fase, bukan sebagai fase terpisah
├── Backend: Leverage OSN knowledge, focus ke engineering practices
├── Projects: Tiered - ada "admission bait" + "real impact" + "portfolio showpiece"
└── Resources: Updated ke 2026 best practices
```

---

# 🎓 YEAR 1: FOUNDATION + PRODUCTION APPS (Sekarang - 52 Minggu)

> **Intensive learning phase sebelum masuk university. Fokus: BUILD THINGS THAT WORK.**

### ⚡️ Flexibility Disclaimer

```
TIMELINE INI BUKAN HARD DEADLINE — INI GUIDELINE.

Prinsip:
├── ❌ "Harus selesai minggu 13" → ✅ "Se口中 selesai quando estiver pronto"
├── ❌ "Telat 2 minggu = gagal" → ✅ "Telat 2 minggu = adjust target"
├── ❌ "Tidak bisa skip minggu" → ✅ "Pahami concepts, tidak harus berurutan"
└── ❌ "1 minggu = 1 minggu" → ✅ "1 phase = ~13 minggu, ±2 minggu acceptable"

Yang PENTING:
1. Paham Konsep (understanding) > tepat Waktu (schedule)
2. working Project > banyak tutorial
3. Consistency > intensity
4. Ada 52 minggu — 2-3 minggu buffer itu normal

Realistis:
├── Week 1-13 (Web): bisa memakan 10-16 minggu tergantung depth
├── Week 14-26 (Mobile): bisa memakan 12-18 minggu
├── Week 27-39 (Backend+AI): bisa memakan 10-15 minggu
└── TOTAL: 40-60 minggu masih on track

If kamu butuh 18 bulan, bukan berarti gagal.
If kamu selesai 9 bulan, justru lebih baik dari expected.
```

## 📊 Phase Overview

```
Minggu 1-13:    Web Full-Stack (React/Next.js)
Minggu 14-26:   Mobile Development (React Native + SwiftUI)
Minggu 27-39:   Backend Engineering + AI Integration
Minggu 40-50:   Capstone Projects + Portfolio
Minggu 51-52:   Buffer/Rest + Year 2 Planning
```

### 📅 52-Week Calendar View

| Phase | Minggu | Durasi | Fokus |
|-------|--------|--------|-------|
| **Phase 1** | 1-13 | 13 minggu | Web Full-Stack |
| **Phase 2** | 14-26 | 13 minggu | Mobile Development |
| **Phase 3** | 27-39 | 13 minggu | Backend + AI |
| **Phase 4** | 40-50 | 11 minggu | Capstones + Portfolio |
| **Buffer** | 51-52 | 2 minggu | Rest + Year 2 Prep |

---

## 🟢 PHASE 1A: MODERN WEB DEVELOPMENT (Minggu 1-13)

### 🎯 Goal: Master React ecosystem + deploy production apps

### Week-by-Week Breakdown:

| Minggu | Topik | Project | Deliverable |
|--------|-------|---------|-------------|
| **1** | HTML5 Semantic + CSS3 Modern | Personal landing page | Live site di GitHub Pages |
| **2** | CSS: Flexbox, Grid, Custom Properties | Responsive dashboard layout | Browser-tested |
| **3** | JavaScript ES2024+ Deep | Console tools + DOM basics | Interactive UI |
| **4** | React Fundamentals | Component library (10 atoms) | Storybook-style docs |
| **5** | React: State + Hooks | Todo app dengan useState/useReducer | Working app |
| **6** | React: useEffect + API Calls | GitHub repos viewer | Real data fetching |
| **7** | React Router + Navigation | Multi-page blog app | Routing working |
| **8** | Next.js 14 App Router | Portfolio v2 dengan SSG | Deployed to Vercel |
| **9** | Server Actions + Database | Blog dengan Prisma + PostgreSQL | CRUD working |
| **10** | Authentication + Security | Full auth flow (NextAuth + JWT) | Secure app |
| **11** | Tailwind CSS v4 + shadcn/ui | Redesign semua apps | Polished UI |
| **12** | Testing + CI/CD | Unit tests + integration tests | 80%+ coverage |
| **13** | **Phase 1 Review** + Portfolio | Rapikan semua project + writeup | Phase 1 complete |

### 🔗 Resources Updated 2026:

| Resource | URL | Why Better |
|----------|-----|------------|
| **The Odin Project** | theodinproject.com | Still best, free, project-driven |
| **React.dev** | react.dev/learn | Official, interactive, 2026 updated |
| **Next.js Official** | nextjs.org/learn | App Router, Server Components |
| **Tailwind CSS** | tailwindcss.com | v4 is game-changer with CSS-first config |
| **shadcn/ui** | ui.shadcn.com | Copy-paste components, customizable |
| **ShipFast** | shipfast.dev | Next.js boilerplate dengan auth/payments already done |

### 💡 AI-Proof Skills di Phase 1:

```javascript
// YANG AI BISA:
// ✅ Generate component dari deskripsi
// ✅ Autocomplete code
// ✅ Translate design ke code (Figma → React)

// YANG ANDA HARUS BISA:
1. decomposeProblem() // pecah masalah besar → komponen kecil
2. evaluateTradeoffs() // Context API vs Zustand vs Redux? Kapan?
3. debugWithoutAI() // DevTools, console.log, breakpoint thinking
4. designArchitecture() // folder structure, data flow, state management
```

---

## 🔵 PHASE 1B: MOBILE DEVELOPMENT (Minggu 14-26)

### 🎯 Goal: Ship apps ke iOS App Store dan Google Play Store

### Mengapa FLUTTER + REACT NATIVE (bukan native Swift/Kotlin)?

```
ARGUMEN UNTUK CROSS-PLATFORM:
├── 1 codebase → iOS + Android (2x reach)
├── React Native dengan Expo = fast iteration
├── Market size Indonesia: Android dominant (80%+)
└── Bridge ke AI lebih mudah (React Native + TensorFlow.js)

ARGUMEN UNTUK SWIFTUI (tetap belajar, Phase 3):
├── Apple ecosystem adalah competitive advantage kamu
├── MacBook M4 = bisa optimize native performance
└── visionOS / watchOS = emerging markets
```

### Week-by-Week: React Native + Expo

| Minggu | Topik | Project | Deliverable |
|--------|-------|---------|-------------|
| **14** | React Native Fundamentals + Expo | "Hello World" di simulator | App running |
| **15** | Core Components + Navigation | Multi-screen app dengan React Navigation | Navigasi works |
| **16** | State Management (Zustand/Redux Toolkit) | Shopping cart dengan state management | State persistent |
| **17** | Native Modules + Device APIs | Camera + Image picker app | Camera access |
| **18** | REST API + GraphQL | News reader app dengan API | Real data |
| **19** | Push Notifications + Offline | Todo app dengan background sync | Notifications work |
| **20** | App Store deployment | Build + submit ke TestFlight + Google Play | Apps submitted |
| **21** | App Store Optimization (ASO) | Research + keywords + screenshots | Optimized listing |

### Week-by-Week: SwiftUI (Bonus untuk Apple Ecosystem)

| Minggu | Topik | Project | Deliverable |
|--------|-------|---------|-------------|
| **22** | Swift + Xcode basics | Swift Playgrounds | Swift熟练 |
| **23** | SwiftUI Fundamentals | "Hello World" di simulator | SwiftUI app |
| **24** | Views, Stacks, State | Resume builder app | UI working |
| **25** | Data persistence (SwiftData) | Journal app | Local storage |
| **26** | **Phase 2 Review** + Integration | Combine RN + SwiftUI learnings | Phase 2 complete |

### 📱 Impact Project Ideas (Universities LOVE these):

```
TIER 1: "Admission Bait" Projects
├── 🏆 Problem-solving app untuk siswa Indonesia (Math/Science)
├── 🏆 Bahasa Indonesia learning app dengan AI tutoring
└── 🏆 Carbon footprint tracker dengan gamification

TIER 2: Real Impact Projects
├── 🚀 Community platform untuk OSN preparation
├── 🚀 Mental health check-in app untuk students
└── 🚀 Local language preservation app

TIER 3: Portfolio Showpieces
├── ⚡ Real-time collaboration whiteboard
├── ⚡ AI-powered study assistant
└── ⚡ Cross-platform habit tracker dengan sync
```

### 🔗 Resources:

| Resource | URL | Notes |
|----------|-----|-------|
| **React Native Expo** | expo.io | Fastest way to build mobile |
| **React Navigation** | reactnavigation.org | v7 is stable |
| **Zustand** | zustand-demo.pmnd.rs | Simple state, no boilerplate |
| **React Native Paper** | reactnativepaper.com | Material Design components |
| **SwiftUI** | hackingwithswift.com | Paul Hudson's 100 Days is best |

---

## 🟣 PHASE 1C: BACKEND ENGINEERING + AI INTEGRATION (Minggu 27-39)

### 🎯 Goal: Build production-grade backend + integrate AI meaningfully

### Mengapa Fase Ini Setelah Web + Mobile?

```
SEQUENCING YANG BENAR:
1. Learn frontend (React) → understand UI + data flow
2. Learn mobile → understand UX constraints
3. THEN learn backend → karena kamu sudah tahu "untuk apa" backend

KENAPA TIDAK DI AWAL:
├── Tanpa frontend understanding, backend terasa abstract
├── Tanpa mobile experience, tidak paham mobile-specific needs
└── OSN sudah taught you: data structures + algorithms = cukup untuk backend basics
```

### Week-by-Week: Backend Engineering

| Minggu | Topik | Project | Deliverable |
|--------|-------|---------|-------------|
| **27** | Node.js Deep Dive | CLI tool (file organizer) | npm package published |
| **28** | Express.js + REST API Design | REST API for mobile app | Full CRUD API |
| **29** | PostgreSQL + Prisma | Database schema + migrations | Production DB |
| **30** | Authentication (JWT + Refresh Tokens) | Secure auth system | Login/register works |
| **31** | Caching + Performance | Redis caching layer | 10x faster queries |
| **32** | Docker + Containerization | Dockerize full-stack app | docker-compose up works |
| **33** | CI/CD + GitHub Actions | Pipeline: lint → test → deploy | Auto-deploy |
| **34** | Monitoring + Observability | Logging + error tracking (Sentry) | Alerts working |

### Week-by-Week: AI Integration (Practical, Not Just API Calls)

| Minggu | Topik | Project | Deliverable |
|--------|-------|---------|-------------|
| **35** | AI Fundamentals + Prompt Engineering | Build CLI AI assistant | Working AI tool |
| **36** | OpenAI API + Function Calling | Study assistant dengan AI tutoring | AI features |
| **37** | Vector Databases + RAG | Private knowledge base app | RAG pipeline |
| **38** | Local AI + Ollama | Offline AI assistant app | Works offline |
| **39** | **Phase 3 Review** + Integration | Connect all pieces together | Phase 3 complete |

### 📚 AI Resources (Updated 2026):

| Resource | URL | Why Essential |
|----------|-----|---------------|
| **Google ML Crash Course** | developers.google.com/machine-learning | Free, high quality |
| **Hugging Face Course** | huggingface.co/learn | transformers + diffusers |
| **LangChain Academy** | langchain.academy | LLM app development |
| **Fast.ai** | fast.ai | Practical deep learning |
| **Chip Huyen's ML Book** | github.com/chiphuyen/machine-learning-systems-design | System design for ML |

### 💡 AI-Proof Skills (Yang AI TIDAK BISA Replace):

```
AI TIDAK BISA:
├── Decide KAPAN pakai AI (vs rule-based vs human judgment)
├── Design AI system architecture
├── Evaluate AI output quality + bias
├── Make AI decisions that align dengan business goals
└── Communicate AI limitations ke non-technical stakeholders

YANG KAMU HARUS Kuasai:
1. AI System Design — bukan cuma "call API"
2. Evaluation Metrics — precision, recall, F1, BLEU, ROUGE
3. Bias Detection — data quality, model fairness
4. Cost Optimization — API costs vs local inference tradeoffs
5. Human-in-the-loop Design — when to trust AI, when to override
```

---

## 🟠 PHASE 1D: CAPSTONE PROJECTS + PORTFOLIO (Minggu 40-50)

### 🎯 Goal: Ship 3 capstone projects yang compelling untuk university applications

### Week-by-Week Breakdown:

| Minggu | Fokus | Aktivitas | Deliverable |
|--------|-------|-----------|-------------|
| **40** | Capstone Planning | Pilih 1-2 capstone + buat SPEC.md | SPEC document |
| **41-42** | Capstone 1: Build | Core features + MVP | MVP launched |
| **43-44** | Capstone 1: Polish | Testing + CI/CD + polish | Production ready |
| **45-46** | Capstone 2: Build | Core features + MVP | MVP launched |
| **47-48** | Capstone 2: Polish + Capstone 3 Start | Testing + polish + plan #3 | Cap 2 done, Cap 3 started |
| **49-50** | Capstone 3 + Portfolio | Final capstone + portfolio writeup | All 3 capstones + portfolio |
| **51-52** | **BUFFER: Rest + Year 2 Planning** | Review + plan next year | Ready for Year 2 |

### 🏆 Capstone Project Tiering:

```
TIER 1: "I got into MIT/Stanford" Level (Pilih 1)
├── 🍎 Full-stack platform dengan 1000+ users (e.g., study group app)
├── 🍎 AI product dengan real business model (e.g., AI tutoring)
└── 🍎 Open source project dengan 500+ GitHub stars

TIER 2: "Strong applicant at NTU/NUS" Level (Pilih 1)
├── 🚀 Mobile app dengan 100+ downloads
├── 🚀 Backend system dengan 10k+ API calls/day
└── 🚀 AI feature di production dengan user feedback

TIER 3: "证明了 passion" Level (Pilih 1)
├── 📱 Contribute ke open source (2+ merged PRs)
├── 📱 Write 3+ technical blog posts
└── 📱 Participate di hackathon (哪怕没赢)
```

### 📋 Suggested Capstone Projects (Impact-Focused):

#### Capstone 1: AI-Powered Learning Platform (Web + Mobile)

```yaml
Problem: Students Indonesia lacks quality personalized learning
Solution: 
  - AI tutor yang adaptif (adjusts to learning pace)
  - Spaced repetition dengan SM-2 algorithm
  - Progress tracking untuk orang tua
Tech Stack:
  - Frontend: Next.js + React Native (shared components)
  - Backend: Express + PostgreSQL + Redis
  - AI: GPT-4o mini + fine-tuned model untuk Indonesian context
  - Infrastructure: Vercel + Railway
Impact Metrics:
  - Pilot dengan 50 students
  - 20% improvement in test scores
  - Featured di local news
```

#### Capstone 2: Environmental Monitoring App (Mobile-first)

```yaml
Problem: Kurang awareness tentang kualitas udara/air di Indonesia
Solution:
  - Crowdsourced air quality data
  - Gamification dengan challenges
  - Integration dengan pemerintah data (BMKG)
Tech Stack:
  - Mobile: React Native + Expo
  - Backend: Node.js + PostgreSQL + Mapbox
  - AI: Predict pollution levels dengan time series
Impact Metrics:
  - 1000+ active users
  - Partnership dengan 1 NGO
  - Presented di climate tech competition
```

#### Capstone 3: Local Language Preservation Platform (AI + Cultural Impact)

```yaml
Problem: Bahasa daerah extinction risk — 70% bisa hilang di 2100
Solution:
  - Crowdsourced translation platform
  - AI-assisted translation (Indonesian ↔ daerah)
  - Audio recording untuk pronunciation preservation
Tech Stack:
  - Frontend: Next.js PWA
  - Backend: PostgreSQL + Prisma
  - AI: Whisper (speech-to-text) + translation model
  - Storage: S3 + Cloudflare R2
Impact Metrics:
  - 500+ words documented
  - Partnership dengan，语言学者
  - Media coverage (Kompas/Detik)
```

### 📂 Portfolio Structure (Yang University Appreciate):

```
📁 Your Portfolio/
├── 📄 README.md (Always updated)
├── 📁 Projects/
│   ├── 📁 capstone-1/ (Full case study)
│   │   ├── PROBLEM.md
│   │   ├── SOLUTION.md
│   │   ├── ARCHITECTURE.md
│   │   ├── DEMO.mp4
│   │   └── IMPACT.md (metrics!)
│   ├── 📁 capstone-2/
│   └── 📁 smaller-projects/
├── 📁 Blog/
│   ├── 🚀 "How I built [X] with [Y]"
│   ├── 🚀 "What I learned from failing [Z]"
│   └── 🚀 "Why [Technology] is overrated/underrated"
└── 📁 Open Source/
    ├── 📁 contributions.md
    └── 📁 your-oss-projects/
```

---

# 📅 YEAR 2-5: DEEPENING + PROFESSIONAL ENGINEER

## Year 2: First Income + Specialization

```
└── Fokus:
    ├── Freelance project pertama (Rp 5-20 juta)
    ├── Intern di startup (remote-friendly)
    ├── Pilih specialization track:
    │   ├── 🅰️ Full-Stack Product Engineer
    │   ├── 🅱️ Mobile-First Engineer
    │   └── 🅾️ AI/ML Engineer
    └── Bangun "第二条曲线" (side income)

└── Projects:
    ├── Client project #1 (paid)
    ├── SaaS side project ( Rp 1-5 juta/month)
    └── Open source contributions (build reputation)
```

## Year 3: Professional Engineer

```
└── Fokus:
    ├── Masuk university (CS/AI focus)
    ├── System design mastery (DDIA book mandatory)
    ├── Team collaboration (code review, agile)
    └── Scale ke 1000+ users

└── Key Skills:
    ├── Distributed systems
    ├── Database at scale
    ├── API design for longevity
    └── Cost optimization
```

## Year 4: Tech Leadership

```
└── Fokus:
    ├── Mentor junior engineers
    ├── Make architectural decisions
    ├── Tech talks (internal + conference)
    └── Build team culture

└── Projects:
    ├── Lead capstone project
    ├── Internal tooling (high leverage)
    └── External speaking (build personal brand)
```

## Year 5: Unreplaceable

```
└── Fokus:
    ├── Principal/Staff Engineer trajectory
    ATAU
    ├── Co-founder / CTO startup
    ATAU
    ├── Premium consulting ( Rp 50-200 juta/bulan)
    └── Teaching / course creation

└── Multiple Income Streams:
    ├── Salary (senior IC)
    ├── Consulting
    ├── Course/saas revenue
    └── Speaking/writing
```

---

# 🎯 PROJECT IMPACT FRAMEWORK

## Bagaimana University Melihat Projects:

```
COMMITTEE MENTALTYY:
├── "Can this student execute?" → Yes, if you have 3+ working apps
├── "Can this student think?" → Yes, if case studies show reasoning
├── "Will this student contribute?" → Yes, if open source + collaboration
├── "Is this student passionate?" → Yes, if projects align dengan interests
└── "Will this student graduate and succeed?" → Yes, if OSN-level problem solving

PROOF HIERARCHY:
1. 📱 Working app in production (hardest to fake)
2. 📝 Detailed case study (shows thinking)
3. 📊 Metrics/impact numbers (shows results)
4. 👥 User testimonials (shows user love)
5. 🐛 Bug reports fixed (shows process)
6. 📖 Blog posts (shows communication)
```

## Projects dengan "Story Value" Tinggi:

```
YANG KEREN DI PAPER:
├── 🏆 "I built X that helps Y people with Z problem"
├── 🏆 "I contributed to open source project X (10k stars)"
├── 🏆 "I won/improved at competition X"
└── 🏆 "I taught myself X and built Y in 2 weeks"

DIHINDARI (waste of time):
├── ❌ "I followed tutorial and built Instagram clone"
├── ❌ "I built 20+ tutorial projects"
├── ❌ "I have 1000+ GitHub contributions (but no meaningful projects)"
└── ❌ "I learned X, Y, Z certifications"
```

---

# 📚 FINAL RESOURCE STACK (2026 Edition)

## Web Development

| Resource | URL | sudah enough |
|----------|-----|--------------|
| The Odin Project | theodinproject.com | Full curriculum |
| React.dev | react.dev/learn | Interactive |
| Next.js Docs | nextjs.org/docs | Official |
| Tailwind CSS | tailwindcss.com | v4 |

## Mobile

| Resource | URL | Notes |
|----------|-----|-------|
| Expo | expo.io | Start here |
| React Native Paper | reactnativepaper.com | Components |
| SwiftUI | hackingwithswift.com | 100 Days |

## Backend

| Resource | URL | Notes |
|----------|-----|-------|
| Node.js Docs | nodejs.org/docs | Official |
| PostgreSQL | postgresql.org/docs | Free |
| Prisma | prisma.io/docs | Best ORM |
| Docker | docker.com | Essential |

## AI/ML

| Resource | URL | Notes |
|----------|-----|-------|
| Fast.ai | fast.ai | Practical |
| Hugging Face | huggingface.co | Models |
| LangChain | langchain.com | LLM Apps |
| Chip Huyen's Book | bit.ly/ml-systems-design | System design |

## System Design

| Resource | URL | Notes |
|----------|-----|-------|
| DDIA | amazon.com | Wajib baca |
| System Design Primer | github.com/donnemartin | GitHub repo |
| High Scalability | highscalability.com | Case studies |

---

# ⚡ RULES FOR SUCCESS

```
1. **Build > Learn > Repeat** — 80% build, 20% learn
2. **Ship every 2 weeks** — App releases train discipline
3. **Document everything** — Case study per project
4. **Get real feedback** — User testing > self-assessment
5. **1-2 hours/day CONSISTENT** — 10 hours/week > 70 hours burnout
6. **AI sebagai accelerator** — "I built X first, then used AI to review"
7. **University prep is NOT the goal** — Real skills are; university is byproduct
8. **OSN skills are leverage** — Use them for algorithm competitions + problem solving
```

---

# 🔄 Quick Reference: What Changed from Original

| Original | Revised | Why |
|----------|---------|-----|
| iOS only | iOS + Android | Indonesia Android-dominant market |
| AI as separate phase | AI integrated throughout | AI is tool, not subject |
| Backend weeks 35-44 | Compressed + leveraged OSN | OSN = backend fundamentals |
| 52 weeks linear | 4 quarters flexible | University prep + life happens |
| General project ideas | Specific impact-focused projects | University want demonstrable impact |
| Generic resources | 2026-specific resources | Best resources evolve |

---

> *"The best time to start was 1 year ago. The second best time is now."*
> *"AI will replace engineers who don't understand. It will amplify those who do."*

**GO BUILD THINGS THAT MATTER. 🔥**
