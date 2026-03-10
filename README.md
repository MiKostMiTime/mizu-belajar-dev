# 🚀 Mizu Belajar Dev — Software Engineering Roadmap

> **Roadmap belajar software engineering yang project-driven, AI-proof, dan future-proof.**
> Didesain untuk anak SMA yang sudah punya CS fundamentals (OSN) dan ingin membangun skill yang TIDAK BISA digantikan AI.

---

## 🛡️ Filosofi: Menjadi AI-Proof Engineer

```
AI/Vibe-Coders bisa:              Kamu harus bisa (yang AI TIDAK bisa):
├── Generate boilerplate code      ├── Arsitektur sistem yang kompleks
├── Autocomplete syntax            ├── Memahami KENAPA, bukan hanya APA
├── Translate requirements to code ├── Debug masalah yang belum pernah ada
├── Write tests from specs         ├── Desain UX yang empatik & manusiawi
└── Copy-paste patterns            ├── Komunikasi & kolaborasi tim
                                   ├── Evaluate trade-offs (scalability vs speed vs cost)
                                   ├── Kreativitas & product thinking
                                   └── Belajar teknologi baru dengan cepat (meta-learning)
```

### 🔑 5 Prinsip Anti-Replacement:
1. **Pahami "KENAPA" di balik setiap kode** — Jangan cuma copy-paste, pahami arsitektur & trade-offs
2. **Build real things for real people** — Portfolio > Sertifikat. User feedback > Tutorial completion
3. **Master the fundamentals, ride the tools** — Framework berubah setiap 2 tahun. CS fundamentals bertahan selamanya
4. **Be a builder, not just a coder** — Product thinking + design + engineering = irreplaceable
5. **Use AI as accelerator, not replacement** — Tulis dulu sendiri → pakai AI untuk review & optimize → pahami perbedaannya

---

## 📌 Konteks Pribadi

| Item | Detail |
|------|--------|
| **Hardware** | MacBook M4 Max 48GB RAM |
| **Design Tool** | Figma |
| **Code Editor (Web)** | PHPStorm (superset of WebStorm) |
| **Code Editor (iOS)** | Xcode |
| **Terminal** | iTerm2 |
| **Browser** | Brave (Chromium — full DevTools) + Safari (cross-browser testing) |
| **CS Fundamentals** | ✅ Sudah punya dari persiapan OSN (algoritma, data structures, problem solving) |
| **ML on device** | Create ML |

---

## 🗂️ Tools Stack

### Install Day One (di iTerm2):
```bash
# 1. Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# 2. Essentials
brew install git node python

# 3. Git config
git config --global user.name "MiKostMiTime"
git config --global user.email "YOUR_EMAIL@example.com"

# 4. SSH key untuk GitHub
ssh-keygen -t ed25519 -C "YOUR_EMAIL@example.com"

# 5. Useful tools (install sesuai fase)
brew install --cask docker        # Fase 4
brew install --cask tableplus     # Fase 4
brew install --cask sf-symbols    # Fase 3
brew install --cask bruno         # Fase 4

# 6. Verify
node --version && npm --version && git --version && python3 --version
```

### PHPStorm Plugins:
- GitHub Copilot, Tailwind CSS, Prettier, ESLint, Prisma, .env files support, GitToolBox

> ⚠️ **Catatan ESLint:** PHPStorm's ESLint plugin **membutuhkan ESLint npm package** yang di-install di dalam project. Tanpa package-nya, plugin tidak bisa berjalan. Install ESLint sebagai dev dependency di **setiap** JavaScript/TypeScript project.

### ESLint Setup (wajib di setiap JS/TS project):
```bash
# Install ESLint sebagai dev dependency
npm install --save-dev eslint

# Inisialisasi konfigurasi ESLint
npx eslint --init
```

Pilihan saat `eslint --init`:
- ✅ **How would you like to use ESLint?** → `To check syntax, find problems, and enforce code style`
- ✅ **What type of modules?** → `JavaScript modules (import/export)` untuk project modern / `CommonJS` untuk Node.js
- ✅ **Which framework?** → sesuaikan (React / None)
- ✅ **Does your project use TypeScript?** → Yes/No sesuai project
- ✅ **Where does your code run?** → Browser / Node sesuai project

Setelah setup, tambahkan script ke `package.json`:
```json
"scripts": {
  "lint": "eslint .",
  "lint:fix": "eslint . --fix"
}
```

Kemudian di PHPStorm: **Settings → Languages & Frameworks → JavaScript → Code Quality Tools → ESLint** → pilih **Automatic ESLint configuration** agar PHPStorm otomatis deteksi dari `node_modules`.

### Workspace Structure:
```
📁 ~/Developer/
├── 📁 web-projects/
├── 📁 ios-projects/
├── 📁 backend-projects/
└── 📁 learning/
```

---

# 📅 ROADMAP 52 MINGGU (Revisi Final)

> **Karena kamu sudah punya CS fundamentals dari OSN**, Fase 4 sekarang berfokus pada backend engineering & system design, BUKAN belajar algoritma dari nol. Waktu yang dihemat dipakai untuk skill yang membuat kamu AI-proof: arsitektur, product thinking, dan building real products.

---

## 🟢 FASE 1: FONDASI WEB + FIRST DEPLOY (Minggu 1–10)

### 📖 Sumber Utama: [The Odin Project](https://theodinproject.com) | Referensi: [MDN Web Docs](https://developer.mozilla.org)

### 🎯 Goal: Bisa bikin web app interaktif dan deploy ke internet

| Minggu | Fokus | 🔨 Project | ✅ Deliverable |
|--------|-------|------------|----------------|
| **1** | HTML semantic + CSS basics + Box Model | **Personal Profile Page** — design di Figma → code | Halaman HTML/CSS live di GitHub Pages |
| **2** | Flexbox + Grid + Responsive Design | **Landing Page responsive** — mobile-first approach | Landing page responsive di semua device |
| **3** | JS Fundamentals — variables, types, conditionals, loops, functions | **Kalkulator** (console dulu → lalu dengan UI) | Kalkulator working di browser |
| **4** | DOM Manipulation + Events | **Rock Paper Scissors** dengan UI + score tracking | Game interaktif |
| **5** | Arrays, Objects, Higher-order functions | **To-Do List** — add, delete, filter, mark complete | CRUD app di browser |
| **6** | ES6+ — arrow functions, destructuring, modules, async/await | **Quiz App** — fetch questions dari Open Trivia API | App yang consume external API |
| **7** | Fetch API + JSON + Error Handling | **Weather App** — lokasi user → tampilkan cuaca + 5-day forecast | Weather app functional |
| **8** | LocalStorage + State Management sederhana | **Bookmark Manager** — save, categorize, search bookmarks | App dengan persistent data |
| **9** | Git mastery — branching, merging, rebasing, PR workflow | Rapikan SEMUA 6 project + proper README setiap repo | 6 repos clean di GitHub |
| **10** | Deployment + Portfolio | **Portfolio Website v1** — showcase semua project + deploy | ✅ **MILESTONE: Portfolio LIVE + 7 projects** |

### 🧠 AI-Proof Skill yang Dibangun di Fase 1:
- Debugging tanpa AI (DevTools mastery)
- Problem decomposition (pecah masalah besar jadi kecil)
- Figma → Code workflow (design thinking)

---

## 🔵 FASE 2: REACT + NEXT.JS FULL-STACK (Minggu 11–22)

### 📖 Sumber: [react.dev/learn](https://react.dev/learn) | [Next.js Learn](https://nextjs.org/learn) | [The Odin Project React](https://theodinproject.com)

### 🎯 Goal: Build & deploy full-stack web application

| Minggu | Fokus | 🔨 Project | ✅ Deliverable |
|--------|-------|------------|----------------|
| **11** | React Basics — components, JSX, props | **UI Component Library** — 10 reusable components | Component set documented |
| **12** | State + Events — useState, conditional rendering | **CV/Resume Builder** — input form → generate printable CV | Working app |
| **13** | useEffect + API fetching in React | **GitHub Profile Viewer** — input username → show repos, stats | App that fetches real data |
| **14** | React Router + Multi-page SPA | **Portfolio v2** — upgrade ke React SPA dengan routing | Portfolio upgraded |
| **15** | Context API + Complex State | **Shopping Cart** — product list, add/remove, quantities, checkout | E-commerce cart working |
| **16** | Custom Hooks + Performance | Refactor projects + buat 3 custom hooks (useFetch, useLocalStorage, useDebounce) | Cleaner codebase + reusable hooks |
| **17** | Next.js — routing, SSR, SSG | **Migrate Portfolio ke Next.js** + add blog section | Portfolio with SSG blog |
| **18** | API Routes + Server Actions | **URL Shortener** — shorten links, track clicks, dashboard | Full-stack CRUD app |
| **19** | Database — Prisma + SQLite → PostgreSQL | **Personal Blog** — write, edit, delete articles + markdown support | Blog with real database |
| **20** | Tailwind CSS + shadcn/ui | Redesign ALL projects dengan Tailwind + consistent design system | Modern, polished UI |
| **21** | Figma Design System → Code | Build **mini design system** di Figma → implement sebagai component library | Design system documented & coded |
| **22** | **🏆 CAPSTONE WEB** | **SaaS App** — Habit Tracker / Budget App / Note-taking app. Full: Figma → Next.js + Tailwind + Prisma + Auth + Deploy Vercel | ✅ **MILESTONE: Full-stack SaaS LIVE with real users** |

### 🧠 AI-Proof Skills di Fase 2:
- **Architecture decisions** — kapan pakai SSR vs SSG vs CSR? Kenapa?
- **System design thinking** — database schema design, API design
- **Product thinking** — build for real users, get feedback, iterate
- **Design engineering** — Figma → Code pipeline yang smooth

---

## 🟣 FASE 3: iOS NATIVE DEVELOPMENT (Minggu 23–34)

### 📖 Sumber: [100 Days of SwiftUI](https://hackingwithswift.com/100/swiftui) | [Apple Dev Tutorials](https://developer.apple.com/tutorials/develop-in-swift)

### 🎯 Goal: Ship iOS app yang berjalan di device sendiri

| Minggu | Fokus | 🔨 Project | ✅ Deliverable |
|--------|-------|------------|----------------|
| **23** | Swift — types, control flow, functions, optionals | 20+ Swift Playground challenges | Swift basics solid |
| **24** | Structs, Classes, Protocols, Enums | **Quiz Game** di Playground | OOP mastery |
| **25** | SwiftUI — Views, Modifiers, Stacks, Layout | **Unit Converter** — weight, length, temperature | First app di simulator |
| **26** | State, Binding, ObservableObject | **Guess the Flag** — quiz game + scoring + animations | Interactive game |
| **27** | Lists, Navigation, Forms | **Expense Tracker** — input, categorize, list, total | Financial app working |
| **28** | Networking — URLSession, JSON, Codable | **News Reader** — fetch real news API + pull to refresh | App with live data |
| **29** | SwiftData (modern persistence) | **Bookworm** — add books, rate, review, persist locally | App with local database |
| **30** | Animations + Gestures + Custom Views | **Polish ALL apps** — micro-interactions, transitions, haptics | Apps feel premium |
| **31** | MapKit + CoreLocation | **Places App** — save favorite locations + show on map | Location-aware app |
| **32** | MVVM Architecture + Clean Code | **Refactor ALL projects ke MVVM** | Clean architecture |
| **33** | Create ML + CoreML integration | **Image Classifier** — train model di Create ML → integrate ke app | On-device ML app |
| **34** | **🏆 CAPSTONE iOS** | **iOS App** — Finance Tracker / Discovery App / Wellness App. Full: Figma → SwiftUI + MVVM + SwiftData + MapKit + Deploy ke TestFlight | ✅ **MILESTONE: iOS app on real device** |

### 🧠 AI-Proof Skills di Fase 3:
- **Platform expertise** — deep understanding of Apple ecosystem (competitive advantage karena punya Mac)
- **On-device ML** — Create ML + CoreML = AI yang berjalan offline, privacy-first
- **UX empathy** — mobile UX itu beda dari web, butuh pemahaman human interaction

---

## 🟠 FASE 4: BACKEND ENGINEERING + SYSTEM DESIGN (Minggu 35–46)

### 📖 Sumber: [freeCodeCamp Backend](https://freecodecamp.org) | [The Odin Project NodeJS](https://theodinproject.com)

### 🎯 Goal: Build production-grade backend + understand system design

> ⚡ Karena OSN sudah cover DSA, fase ini fokus ke **engineering skills** yang bikin kamu irreplaceable

| Minggu | Fokus | 🔨 Project / Aktivitas | ✅ Deliverable |
|--------|-------|------------------------|----------------|
| **35** | Node.js deep-dive — runtime, event loop, streams, modules | **CLI Tool** — file organizer / markdown converter / project scaffolder | CLI tool published di npm |
| **36** | Express.js + REST API design + API documentation | **REST API** untuk web capstone + Swagger docs | Documented API |
| **37** | PostgreSQL + Prisma ORM + Database design | **Database schema design** + migrations + seed data | Production-ready DB |
| **38** | Authentication & Authorization — JWT, OAuth 2.0, sessions | **Auth system** — register, login, roles, protected routes, refresh tokens | Secure auth system |
| **39** | Testing — unit tests, integration tests, E2E | **Test suite** untuk API — Jest + Supertest + coverage report | 80%+ test coverage |
| **40** | Error handling, logging, monitoring | Add **structured logging + error handling** ke semua APIs | Production-grade error handling |
| **41** | Docker + Docker Compose | **Containerize** full-stack app (frontend + backend + database) | docker-compose up → everything runs |
| **42** | CI/CD — GitHub Actions | **Pipeline** — lint → test → build → deploy otomatis saat push | Automated deployment |
| **43** | System Design Fundamentals — caching, load balancing, message queues, microservices | Study + **design doc** untuk grand capstone (architecture diagram, tech decisions, trade-offs) | Architecture document |
| **44** | Security — OWASP Top 10, rate limiting, input validation, CORS | **Security audit** semua project + fix vulnerabilities | Hardened applications |
| **45-46** | **🏆 GRAND CAPSTONE** | **Production-grade Full-Stack App** — Multi-user app with: Auth + Database + API + Tests + Docker + CI/CD + Monitoring. Bisa jadi: Project management tool / Marketplace / Social platform | ✅ **MILESTONE: Production-grade app with DevOps** |

### 🧠 AI-Proof Skills di Fase 4:
- **System design** — AI bisa generate code, tapi tidak bisa design arsitektur yang scalable
- **Security mindset** — understanding attack vectors & defensive programming
- **Testing culture** — AI generates code, humans verify correctness
- **DevOps thinking** — infrastructure, deployment, monitoring = high-value skills
- **Trade-off evaluation** — "should we use microservices or monolith?" requires human judgment

---

## 🔴 FASE 5: AI INTEGRATION + SPECIALIZATION + LAUNCH (Minggu 47–52)

### 📖 Sumber: [Kaggle Learn](https://kaggle.com/learn) | [Google ML Crash Course](https://developers.google.com/machine-learning/crash-course) | [3Blue1Brown](https://youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi)

### 🎯 Goal: Integrate AI into your apps + professional launch

| Minggu | Fokus | 🔨 Project / Aktivitas | ✅ Deliverable |
|--------|-------|------------------------|----------------|
| **47** | AI/ML Foundations — 3Blue1Brown + Kaggle Learn (Intro to ML + Intermediate ML) | **Kaggle mini-project** — prediction model + submit to competition | ML model + Kaggle submission |
| **48** | Practical AI Integration — LLM APIs (OpenAI/local models) + Create ML | **Add AI feature ke salah satu capstone** — smart search / content suggestion / image classification | AI-powered feature in production |
| **49** | Open Source Contribution | Find 2-3 "good first issue" → submit PR → get merged | **Merged PR in open source project** |
| **50** | Portfolio v3 Final — case studies, blog posts | **Portfolio production-ready** — setiap capstone punya case study (problem → solution → results) | Portfolio that tells stories |
| **51** | Professional presence + content | GitHub Profile README + 2 technical blog posts + LinkedIn optimized | Professional online presence |
| **52** | **RETROSPECTIVE + YEAR 2 PLANNING** | Review semua yang dipelajari + plan specialization untuk tahun depan | ✅ **MILESTONE AKHIR: 17+ projects, 4 capstones, portfolio live, open source contributor** |

### 🧠 AI-Proof Skills di Fase 5:
- **AI as a tool, not a crutch** — you decide WHEN and HOW to use AI
- **Communication** — writing case studies, blog posts, explaining decisions
- **Open source collaboration** — working with real teams, real codebases
- **Product storytelling** — not just "I built this" but "here's the problem I solved and why it matters"

---

# 🔭 ROADMAP 5 TAHUN (Long-Term Anti-Replacement Strategy)

```
TAHUN 1 (Roadmap di atas)
├── Web Full-Stack (React/Next.js)
├── iOS Native (Swift/SwiftUI)
├── Backend Engineering + DevOps
├── AI/ML Integration
└── Output: 17+ projects, 4 capstones, portfolio, open source

TAHUN 2: DEPTH + FIRST INCOME
├── TypeScript mastery (wajib)
├── Pilih 1 spesialisasi utama:
│   ├── 🅰️ Full-Stack Product Engineer → Advanced React, System Design, SaaS
│   ├── 🅱️ Apple Platform Engineer → visionOS, watchOS, advanced Swift
│   └── 🅾️ AI Engineer → Python deep-dive, LLM apps, RAG, fine-tuning
├── Freelance project pertama / magang
├── Build 1 product with paying users
└── Output: Specialization + first income from coding

TAHUN 3: PROFESSIONAL ENGINEER
├── Masuk kuliah (CS/SE) atau intensive self-study
├── Advanced System Design (distributed systems, databases at scale)
├── Cloud platform (AWS/GCP — pick one, go deep)
├── Team collaboration (code review, agile, mentoring)
├── Build product that scales to 1000+ users
└── Output: Professional experience + product with real traction

TAHUN 4: T-SHAPED EXPERTISE
├── Deep in 1 domain + broad across many
├── Emerging tech that humans will lead:
│   ├── AI/Human collaboration patterns
│   ├── AR/VR (Apple Vision Pro / spatial computing)
│   ├── Edge computing + privacy-first architecture
│   └── Developer tooling & infrastructure
├── Tech leadership: mentoring juniors, tech talks, writing
└── Output: Known expert in 1-2 domains + leadership skills

TAHUN 5: UNREPLACEABLE
├── You can now:
│   ├── Architect complex systems end-to-end
│   ├── Lead teams and make technical decisions
│   ├── Evaluate and adopt ANY new technology rapidly
│   ├── Build products from 0 → users → revenue
│   └── Teach and mentor others
├── Career paths:
│   ├── 🏢 Senior Engineer at top company
│   ├── 🚀 Co-founder / CTO of startup
│   ├── 💼 Premium freelance / consulting
│   └── 🎓 Research / advanced studies
└── Output: Engineer who shapes technology, not just uses it
```

---

# 📊 Final Project Output Summary

| # | Project | Tech Stack | Fase |
|---|---------|------------|------|
| 1 | Personal Profile Page | HTML/CSS | 1 |
| 2 | Landing Page | CSS Flexbox/Grid | 1 |
| 3 | Rock Paper Scissors | JavaScript + DOM | 1 |
| 4 | To-Do List | JavaScript | 1 |
| 5 | Quiz App | JS + API | 1 |
| 6 | Weather App | JS + API + LocalStorage | 1 |
| 7 | Bookmark Manager | JS + LocalStorage | 1 |
| 8 | Portfolio v1 | HTML/CSS/JS | 1 |
| 9 | CV/Resume Builder | React | 2 |
| 10 | Shopping Cart | React + Context | 2 |
| 11 | URL Shortener | Next.js + API Routes | 2 |
| 12 | Personal Blog | Next.js + Prisma + DB | 2 |
| 13 | **🏆 Capstone: SaaS Web App** | Next.js + Tailwind + Prisma + Auth + Vercel | 2 |
| 14 | Expense Tracker iOS | SwiftUI + SwiftData | 3 |
| 15 | News Reader iOS | SwiftUI + URLSession | 3 |
| 16 | Image Classifier | SwiftUI + Create ML + CoreML | 3 |
| 17 | **🏆 Capstone: iOS App** | Swift + MVVM + SwiftData + MapKit | 3 |
| 18 | CLI Tool | Node.js (published to npm) | 4 |
| 19 | REST API + Auth + Tests | Express + PostgreSQL + Jest | 4 |
| 20 | **🏆 Grand Capstone: Full-Stack** | Next.js + Express + PostgreSQL + Docker + CI/CD | 4 |
| 21 | AI/ML Mini Project | Python + Kaggle | 5 |
| 22 | **Portfolio Final** | Next.js + case studies | 5 |

---

# 📋 Resource yang Dipakai (Gratis & Terkurasi)

| Kategori | Sumber | Link |
|----------|--------|------|
| **Web Full-Stack** | The Odin Project | [theodinproject.com](https://theodinproject.com) |
| **React** | React Official Tutorial | [react.dev/learn](https://react.dev/learn) |
| **Next.js** | Next.js Learn | [nextjs.org/learn](https://nextjs.org/learn) |
| **iOS/Swift** | 100 Days of SwiftUI | [hackingwithswift.com](https://hackingwithswift.com/100/swiftui) |
| **iOS/Swift** | Apple Developer Tutorials | [developer.apple.com](https://developer.apple.com/tutorials/develop-in-swift) |
| **Backend** | freeCodeCamp Backend | [freecodecamp.org](https://freecodecamp.org) |
| **AI/ML** | Kaggle Learn | [kaggle.com/learn](https://kaggle.com/learn) |
| **AI/ML** | Google ML Crash Course | [developers.google.com](https://developers.google.com/machine-learning/crash-course) |
| **AI/ML Visual** | 3Blue1Brown Neural Networks | [YouTube Playlist](https://youtube.com/playlist?list=PLZHQObOWTQDNU6R1_67000Dx_ZCJB-3pi) |
| **Git/GitHub** | GitHub Skills | [skills.github.com](https://skills.github.com) |
| **Referensi** | MDN Web Docs | [developer.mozilla.org](https://developer.mozilla.org) |
| **Algorithm Visual** | VisuAlgo | [visualgo.net](https://visualgo.net) |

---

# ⚡ Rules for Myself

1. **80% Build, 20% Learn** — Jangan jatuh ke tutorial hell
2. **1-2 jam/hari konsisten** — Lebih baik dari 10 jam sekali seminggu
3. **AI Rule: Code first 15 min → AI assist → Understand the diff** — Jangan langsung minta AI
4. **Every project gets a README** — Document what you built and why
5. **Push to GitHub EVERY DAY** — Green squares = proof of consistency
6. **Design in Figma BEFORE coding** — Think before you type
7. **Get feedback from real people** — Show your projects, ask for criticism
8. **When stuck > 30 min: take a break, then ask** — Don't burn out

---

# 🔄 Strategi Adaptasi di Tengah Perkembangan Teknologi yang Pesat

> *Teknologi berubah setiap 2–3 tahun. Engineer yang survive bukan yang tahu semua tool, tapi yang tahu cara belajar tool baru dengan cepat.*

## 🧠 Pola Pikir (Mindset) yang Harus Dibangun

```
Cara SALAH:                          Cara BENAR:
├── Hafal setiap framework           ├── Pahami KONSEP di balik framework
├── Ikut setiap hype teknologi       ├── Evaluasi teknologi secara kritis
├── Tutorial satu per satu          ├── Build project nyata → pelajari sesuai kebutuhan
├── Belajar saat ada waktu           ├── Jadwalkan 1–2 jam/hari, konsisten
└── Tunggu "siap" sebelum mulai      └── Ship fast, iterate, improve
```

## 🗺️ Framework Evaluasi Teknologi Baru

Sebelum invest waktu belajar teknologi baru, tanyakan ini:

| Pertanyaan | Indikator Layak Dipelajari |
|------------|---------------------------|
| **Masalah apa yang dipecahkan?** | Ada pain point nyata yang kamu rasakan |
| **Siapa yang pakai di production?** | Big companies atau banyak open source project |
| **Komunitas seberapa aktif?** | GitHub stars tren naik, forum aktif, update rutin |
| **Apakah fundamentals yang sudah ku punya berlaku di sini?** | Jika ya → learning curve lebih pendek |
| **Apakah ada job market-nya?** | Cek LinkedIn/job board untuk 2–3 tahun ke depan |

## ⚡ Framework Belajar Cepat (Meta-Learning)

### 1. The 20% Rule — Cukup 20% untuk Produktif
Dalam teknologi baru, **20% konsep sering cover 80% use cases**. Mulai dari:
- Official "Getting Started" / "Tutorial" resmi
- Build 1 project kecil yang mencerminkan real-world use case
- Expand pengetahuan sesuai kebutuhan project

### 2. Feynman Technique — Uji Pemahaman
1. Pelajari konsep
2. Jelaskan dengan bahasa sendiri seolah mengajar orang lain
3. Identifikasi bagian yang tidak bisa dijelaskan → itu gap yang harus diisi
4. Sederhanakan penjelasan sampai bisa dipahami anak SMA

### 3. Spaced Repetition — Lawan Lupa
- Ulangi materi di interval yang makin panjang: 1 hari → 3 hari → 1 minggu → 1 bulan
- Gunakan Anki (offline) untuk flashcard teknis

### 4. Deliberate Practice — Latihan Terarah
- Jangan hanya re-read / re-watch → praktek langsung
- Identifikasi weakness → fokus latihan di situ
- Cari feedback dari code review, mentor, atau komunitas

## 📡 Cara Tetap Update Tanpa Tenggelam dalam Informasi

```bash
# Weekly routine (max 30 menit/minggu):
1. Cek GitHub Trending (github.com/trending) → lihat apa yang naik
2. Baca 1 newsletter teknis: bytes.dev / tldr.tech / javascriptweekly.com
3. Scan changelog/release notes tool yang sedang kamu pakai
4. Follow 3–5 engineer senior di X/Twitter atau blog pribadi mereka

# Monthly routine (max 2 jam/bulan):
1. Baca 1 engineering blog post dari: engineering.spotify.com, netflixtechblog.com, atau martinfowler.com
2. Review: apakah skill yang sedang kupelajari masih relevan?
3. Update roadmap jika ada teknologi yang worth diprioritaskan
```

---

# 🔌 Belajar Tanpa Akses Internet

> *Koneksi internet bisa hilang. Tapi kalau kamu sudah siapkan environment belajar offline, progress tidak pernah berhenti.*

## 📥 Persiapan Offline — Download Sebelum Tidak Ada Internet

### Dokumentasi Offline (Wajib Download)

| Tool | Cara Download Offline | Ukuran Perkiraan |
|------|----------------------|-----------------|
| **Dash** (macOS) | [kapeli.com/dash](https://kapeli.com/dash) — download docsets pilihan | 50 MB – 2 GB |
| **MDN Web Docs** | Di Dash: tambahkan docset "MDN" | ~200 MB |
| **DevDocs** | [devdocs.io](https://devdocs.io) → Settings → pilih docs → enable offline | ~100–500 MB |
| **Node.js docs** | Di Dash atau `npm install -g node-man` | ~10 MB |
| **Swift docs** | Otomatis tersedia di Xcode offline | Included |
| **React docs** | Di Dash: tambahkan docset "React" | ~5 MB |

> 💡 **Dash** adalah investasi terbaik untuk developer macOS — download sekali, semua docs tersedia offline, terintegrasi dengan PHPStorm dan Xcode.

### Kursus & Video Offline

```bash
# YouTube downloader (legal untuk personal use):
brew install yt-dlp

# Download seluruh playlist:
yt-dlp -f "bestvideo[height<=1080]+bestaudio" \
  --write-sub --sub-lang id,en \
  "https://www.youtube.com/playlist?list=PLAYLIST_ID"

# Download channel/playlist favorit sebelum tidak ada internet:
# - 3Blue1Brown (matematika & neural networks)
# - Fireship (quick tech overviews)
# - Theo (t3.gg) — web dev modern
# - The Primeagen — engineering mindset
# - Hacking with Swift (tutorial iOS)
```

### Books & Reading Material Offline

```bash
# Download e-book gratis yang legal:
# - "You Don't Know JS" series: github.com/getify/You-Dont-Know-JS
# - "Eloquent JavaScript": eloquentjavascript.net (ada versi PDF)
# - "The Pragmatic Programmer" — beli fisik/digital
# - "Clean Code" — beli fisik/digital
# - "Designing Data-Intensive Applications" — beli fisik/digital

# Clone dokumentasi/buku open source ke lokal:
git clone https://github.com/getify/You-Dont-Know-JS
git clone https://github.com/ryanmcdermott/clean-code-javascript
```

### Repository & Source Code Offline

```bash
# Clone semua repo yang mungkin dibutuhkan:
mkdir ~/Developer/offline-refs && cd ~/Developer/offline-refs

# Framework source code (untuk baca ketika stuck):
git clone --depth=1 https://github.com/facebook/react
git clone --depth=1 https://github.com/vercel/next.js
git clone --depth=1 https://github.com/tailwindlabs/tailwindcss

# Best practices & patterns:
git clone https://github.com/goldbergyoni/nodebestpractices
git clone https://github.com/airbnb/javascript
git clone https://github.com/kamranahmedse/developer-roadmap

# Algoritma & data structures reference:
git clone https://github.com/trekhleb/javascript-algorithms
```

## 🛠️ Setup Development Environment Offline Penuh

```bash
# Pastikan semua sudah diinstall dan bisa run TANPA internet:

# 1. Node.js + npm (sudah offline setelah install)
node --version && npm --version

# 2. npm offline cache — install package dulu saat ada internet
npm install <package>  # otomatis di-cache di ~/.npm

# Install ulang dari cache tanpa internet:
npm install --prefer-offline

# 3. Homebrew offline (untuk tools yang sudah pernah di-download)
brew install --formula git  # gunakan cache jika ada

# 4. Docker images — pull dulu saat ada internet
docker pull node:20-alpine
docker pull postgres:16
docker pull redis:alpine

# 5. Xcode — download simulator & additional components saat online
# Xcode → Settings → Platforms → download semua yang dibutuhkan

# 6. CocoaPods / Swift Package Manager
# Resolve dependencies saat online → commit Package.resolved
# Offline install: swift package resolve --only-use-versions-from-resolved-file
```

## 📚 Bahan Belajar Offline yang Bisa Didownload

### Cheat Sheets (Print atau Simpan Lokal)

```
~/Developer/learning/cheatsheets/
├── git-cheatsheet.pdf          # github.com/github/training-kit
├── html5-cheatsheet.pdf        # htmlcheatsheet.com
├── css-tricks-almanac.pdf      # css-tricks.com/almanac
├── javascript-cheatsheet.pdf   # javascript.info (ada PDF)
├── regex-cheatsheet.pdf        # quickref.me/regex
├── vim-cheatsheet.pdf          # jika pakai vim
├── sql-cheatsheet.pdf          # sqltutorial.org/sql-cheat-sheet
└── docker-cheatsheet.pdf       # dockerlabs.collabnix.com
```

### Interactive Learning Offline

| Tool | Kegunaan | Install |
|------|---------|---------|
| **Anki** | Flashcard spaced repetition | [apps.ankiweb.net](https://apps.ankiweb.net) |
| **Obsidian** | Personal knowledge base | [obsidian.md](https://obsidian.md) |
| **Excalidraw** (desktop) | System design diagram offline | `brew install --cask excalidraw` |
| **Zeal** (alternatif Dash, gratis) | Offline docs viewer | [zealdocs.org](https://zealdocs.org) |

---

# 📚 Sumber Belajar Berkualitas & Efektif

> *Bukan yang paling banyak resources yang menang, tapi yang paling fokus dan konsisten menggunakannya.*

## 🥇 Tier 1: Resources Terbaik Per Kategori

### Web Development

| Resource | Tipe | Offline? | Kenapa Bagus |
|----------|------|---------|-------------|
| **The Odin Project** | Kurikulum gratis | ❌ (tapi bisa clone) | Project-driven, community strong, kurikulum terarah |
| **javascript.info** | Book/web | ✅ PDF tersedia | Paling lengkap dan mendalam untuk JavaScript modern |
| **MDN Web Docs** | Referensi | ✅ via Dash | Official, akurat, selalu up-to-date |
| **CSS-Tricks** | Blog/guide | ❌ | Practical CSS dari practitioner |
| **web.dev** (Google) | Guides | Sebagian | Best practices dari Google engineers |

### React & Next.js

| Resource | Tipe | Offline? | Kenapa Bagus |
|----------|------|---------|-------------|
| **react.dev** | Docs resmi | ✅ via Dash | Docs terbaik, ada interactive examples |
| **Next.js Docs** | Docs resmi | ✅ via Dash | Official, lengkap dengan examples |
| **Josh W Comeau** (blog) | Blog | Sebagian cache | Penjelasan visual, mendalam, praktis |
| **ByteGrad YouTube** | Video | ✅ yt-dlp | Real-world Next.js patterns |

### iOS / Swift

| Resource | Tipe | Offline? | Kenapa Bagus |
|----------|------|---------|-------------|
| **100 Days of SwiftUI** | Kurikulum | Sebagian | Project-driven, Paul Hudson sangat jelas menjelaskan |
| **Swift.org** | Docs resmi | ✅ via Dash | Official Swift language reference |
| **Apple Developer Docs** | Docs resmi | ✅ via Xcode | Framework reference lengkap, built-in di Xcode |
| **Hacking with Swift** | Blog/buku | Sebagian | Real-world patterns, tips yang tidak ada di docs resmi |

### Backend & System Design

| Resource | Tipe | Offline? | Kenapa Bagus |
|----------|------|---------|-------------|
| **Node.js Docs** | Docs resmi | ✅ via Dash | Official, precise |
| **PostgreSQL Docs** | Docs resmi | ✅ via Dash | Paling komprehensif untuk SQL |
| **Designing Data-Intensive Applications** | Buku | ✅ (beli) | Bible-nya system design, wajib baca |
| **System Design Primer** | GitHub repo | ✅ clone | [github.com/donnemartin/system-design-primer](https://github.com/donnemartin/system-design-primer) |
| **High Scalability** (blog) | Blog | ❌ | Real case studies dari production systems |

### Computer Science Fundamentals

| Resource | Tipe | Offline? | Kenapa Bagus |
|----------|------|---------|-------------|
| **CS50 (Harvard)** | Video course | ✅ download | Fundamentals terbaik, gratis, berkualitas tinggi |
| **CLRS** (Introduction to Algorithms) | Buku | ✅ (beli) | Reference DSA paling authoritative |
| **Neetcode.io** | Video + problems | Sebagian | Paling efektif untuk DSA interview prep |
| **VisuAlgo** | Visualisasi | ❌ | Visual banget untuk algoritma & data structures |

## 🧰 Stack Belajar Efektif (Bukan Banyak, tapi Tepat)

```
PRINSIP: 1 sumber utama per topik + 1 referensi per topik
         Jangan buka 10 tutorial sekaligus → selesaikan 1 dulu

Per Fase, gunakan:
┌─────────────────────────────────────────────────────────┐
│  SUMBER UTAMA           REFERENSI           PRAKTEK     │
│  (ikuti kurikulum)      (ketika stuck)      (wajib)     │
│                                                         │
│  The Odin Project    →  MDN / javascript.info →  BUILD  │
│  react.dev           →  Josh W Comeau blog    →  BUILD  │
│  100 Days SwiftUI    →  Apple Docs / Xcode    →  BUILD  │
│  Buku DDIA           →  System Design Primer  →  DESIGN │
└─────────────────────────────────────────────────────────┘
```

## 📖 Daftar Buku Wajib Baca (Prioritas Berdasarkan Fase)

### Fase 1–2 (Baca sambil belajar):
- **"Eloquent JavaScript"** — Marijn Haverbeke (gratis online, PDF tersedia)
- **"You Don't Know JS"** series — Kyle Simpson (gratis di GitHub)
- **"The Pragmatic Programmer"** — Andrew Hunt & David Thomas ⭐ prioritas tinggi

### Fase 3–4 (Baca sambil belajar):
- **"Clean Code"** — Robert C. Martin (wajib)
- **"Designing Data-Intensive Applications"** — Martin Kleppmann ⭐ prioritas tinggi
- **"The Phoenix Project"** — Gene Kim (DevOps & engineering culture)

### Fase 5 & seterusnya:
- **"A Philosophy of Software Design"** — John Ousterhout
- **"Staff Engineer"** — Will Larson
- **"The Manager's Path"** — Camille Fournier (untuk yang mau ke leadership)

## 🎯 Teknik Belajar yang Terbukti Efektif

### Build-Measure-Learn Loop

```
1. BUILD kecil dulu → jangan tunggu paham semua
2. STUCK → cari di docs resmi DULU (bukan langsung Google/AI)
3. Masih stuck 30 menit → cari di StackOverflow / GitHub Issues
4. Masih stuck → tanya di komunitas / pakai AI
5. SETELAH solved: tulis di Obsidian / catatan pribadi → kamu sudah belajar itu
```

### Active Recall vs Passive Consumption

```
❌ Passive (tidak efektif):
- Re-read tutorial berkali-kali
- Menonton video tanpa praktek
- Copy-paste code tanpa mengerti

✅ Active (efektif):
- Tutup tutorial → coba implement dari memori
- Jelaskan konsep ke diri sendiri (Feynman)
- Build variasi dari contoh yang sudah ada
- Buat test untuk kode yang kamu tulis
```

### Interleaving — Campur Topik

```
Daripada belajar 1 topik 8 jam berturut-turut:
→ Belajar topik A 1 jam → topik B 1 jam → kembali A → kembali B

Ini counter-intuitive tapi terbukti meningkatkan retensi jangka panjang.
Dalam roadmap ini, setiap minggu sudah dirancang dengan variation supaya otak tetap aktif.
```

## 🗃️ Sistem Manajemen Pengetahuan Pribadi (PKM)

Buat "Second Brain" di Obsidian (offline-first):

```
📁 ~/Developer/learning/obsidian-vault/
├── 📁 concepts/            # Penjelasan konsep teknis dengan kata-kata sendiri
│   ├── javascript-closures.md
│   ├── react-reconciliation.md
│   └── database-indexing.md
├── 📁 snippets/            # Code snippets yang sering dipakai
├── 📁 til/                 # "Today I Learned" — satu entry per hari
├── 📁 resources/           # Link & catatan resource yang sudah dikonsumsi
└── 📁 projects/            # Catatan teknis per project
```

> 💡 Setiap kali belajar sesuatu yang baru, **tulis dengan kata-kata sendiri** di vault ini. Satu paragraph saja cukup. Dalam 1 tahun, kamu punya knowledge base pribadi yang jauh lebih berguna dari ratusan bookmark yang tidak pernah dibuka lagi.

---

# 📈 Weekly Progress Tracking

Track progress di [Issues](https://github.com/MiKostMiTime/mizu-belajar-dev/issues) — buat comment setiap minggu:

```markdown
## Week X — [Fase Y]
**Fokus:** [Topik minggu ini]
**Project:** [Nama project]
**Link:** [GitHub repo link]
**What I learned:** [3 bullet points]
**Blockers:** [Apa yang sulit]
**Next week:** [Rencana]
```

---

> *"The best way to predict the future is to build it."* — Alan Kay

> *"AI will replace coders who can't think. It will amplify engineers who can."*

**Mulai dari Minggu 1. Jangan tunggu sempurna. Mulai sekarang. 🔥**