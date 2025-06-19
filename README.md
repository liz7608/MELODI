# 🖥️ Tech Stack

## Overview

Our SaaS platform empowers independent musicians by offering a project management tool tailored for creative workflows. It includes high quality databasing tools, media-rich integrations (Spotify, Pinterest), audio processing, and a visual canvas for moodboarding and asset organization.

---

## 🚀 Frontend

- **Framework**: [React](https://react.dev/learn/installation) (with React Native for mobile support)  
  🛠 Front-end development tool; Code in JavaScript  

- **Drag-and-Drop UI**: [`react-beautiful-dnd`](https://github.com/atlassian/react-beautiful-dnd)  
  🛠 UI Builder for React  

- **Real-Time Collaboration**: [Supabase](https://supabase.com/docs/guides/cron/install)  
  🛠 Tracks real-time updates for user-made edits  

- **Visual Canvas**: Custom-built drag-and-drop grid canvas  
  - Libraries: [Konva.js](https://konvajs.org/) or [fabric.js](http://fabricjs.com/)  
    🛠 Creating visual canvases, similar to Figma or Milanote  

- **Audio Player UI**: [wavesurfer.js](https://wavesurfer-js.org/) or [howler.js](https://howlerjs.com/)  
  🛠 Displays waveform; more just for visuals  

---

## 🧠 Backend

- **API Development**: [Node.js](https://nodejs.org/en/download) (with [Express](https://expressjs.com/)) or [Python FastAPI](https://fastapi.tiangolo.com/)  
  🛠 Backend language  

- **Database**:
  - [PostgreSQL](https://www.postgresql.org/download/)  
    🛠 Structured database; rows and columns; typically for text, memos, and sheets  
  - [MongoDB](https://www.mongodb.com/try/download/community)  
    🛠 Unstructured database; for free-form content like media  

- **Authentication & Realtime Backend**: [Firebase Auth](https://firebase.google.com/docs/auth) + [Firebase Firestore](https://firebase.google.com/products/firestore) or [Supabase](https://supabase.com/)  
  🛠 User authentication  

- **Audio Processing API**:
  - Server-side rendering: Reverb, EQ, Compression  
  - Tools: [FFmpeg](https://ffmpeg.org/), [SoX](http://sox.sourceforge.net/), [`audiomass`](https://github.com/pkalogiros/audiomass), [`Tone.js`](https://tonejs.github.io/)  
    🛠 Renders audio for processing  

---

## 🔌 Third-Party Integrations

### Via [Zapier](https://zapier.com/) or [Make.com](https://www.make.com/):

🛠 Automation/integration between our platform and third-party software

- **Pinterest**: Pull inspiration images or feeds into user boards  
- **Spotify**:
  - Import related artist data  
  - Fetch track/playlist metadata  
  - Embed Spotify players in canvas or notes  

---

## 📁 File Management & Media

- **Cloud Storage**: [Firebase Storage](https://firebase.google.com/products/storage) or [AWS S3](https://aws.amazon.com/s3/)  
  🛠 Storage for all assets  

- **Transcoding**: [FFmpeg](https://ffmpeg.org/) or integration with [Dolby.io](https://dolby.io/communications/pricing/)  
  ⚠️ *SAVE FOR FUTURE DATE:* Audio transcoding for higher quality files  

---

## 🛠 Infrastructure & DevOps

- **Frontend Hosting**: [Vercel](https://vercel.com/)  
  🛠 Vercel used to build the web platform  

- **Backend Hosting**: [Render](https://render.com/) or [Heroku](https://www.heroku.com/)  
  🛠 Render or Heroku for backend  

- **CI/CD**: [GitHub Actions](https://github.com/features/actions)  
  🛠 GitHub Actions for automation  

- **Monitoring**: [LogRocket](https://logrocket.com/) (frontend), [Sentry](https://sentry.io/) (backend)  
  ⚠️ *SAVE FOR FUTURE DATE:* CRM-like tools for debugging  

---

## 🧪 Planned MVP Features

| Feature                 | Stack / Tooling                                     |
|------------------------|-----------------------------------------------------|
| Drag-and-drop interface| React + `react-beautiful-dnd`                       |
| Real-time updates      | WebSockets / Firebase                               |
| Pinterest integration  | Zapier/Make → Pinterest API                         |
| Spotify integration    | Zapier/Make → Spotify API                           |
| Audio editing          | `ffmpeg`, `Tone.js`, or `Web Audio API`             |
| Canvas/Moodboard       | `Konva.js`, `fabric.js`, or `react-flow`            |
| Authentication         | Firebase Auth                                       |
| Database               | PostgreSQL (structured) + MongoDB (unstructured)    |

---

## 💼 Tech Stack with Costs, Links, and Notes

| Category           | Service/Tool                                   | Free Tier | Est. Monthly Cost | Link                                         | Notes                                                                 |
|--------------------|------------------------------------------------|-----------|-------------------|----------------------------------------------|-----------------------------------------------------------------------|
| Frontend Hosting   | Vercel                                          | ✅        | $0–$20            | [vercel.com](https://vercel.com/)            | Free for hobby/dev. Pro adds analytics & team tools.                 |
| Backend Hosting    | Render / Railway                                | ✅        | $7–$25            | [render.com](https://render.com/), [railway.app](https://railway.app/) | Free tier exists; paid plans from $7.                                 |
| Database           | Supabase (PostgreSQL)                           | ✅        | $0–$25            | [supabase.com](https://supabase.com/)        | Free to 500MB; backups and compute scale with cost.                   |
|                    | MongoDB Atlas                                   | ✅        | $0–$30            | [mongodb.com](https://www.mongodb.com/atlas) | Free M0 tier; production pricing scales quickly.                      |
| Auth               | Firebase Auth                                   | ✅        | $0–$20            | [firebase.google.com](https://firebase.google.com/) | Free up to 10K monthly verifications.                                |
| Storage            | Firebase Storage / AWS S3                       | ✅        | $5–$20            | [firebase.google.com](https://firebase.google.com/), [aws.amazon.com](https://aws.amazon.com/s3) | Firebase is good for small media. S3 scales better.                  |
| Realtime Backend   | Firebase Firestore                              | ✅        | $0–$25            | [firebase.google.com](https://firebase.google.com/) | Free to 50K reads/day; be careful with sync-heavy flows.             |
| Integrations       | Zapier                                          | ✅        | $0–$19            | [zapier.com](https://zapier.com/)            | Free 100 tasks/month. Starter = multistep zaps.                       |
|                    | Make.com                                        | ✅        | $0–$16            | [make.com](https://www.make.com/)            | Free for 1,000 ops/month. Basic plan scales up.                      |
| Audio Processing   | FFmpeg / SoX                                    | ✅        | $0 (infra only)   | [ffmpeg.org](https://ffmpeg.org/), [sox.sourceforge.net](http://sox.sourceforge.net/) | Open source; cost is compute-based only.                             |
| Canvas / Visuals   | Konva.js / Fabric.js                            | ✅        | $0                | [konvajs.org](https://konvajs.org/), [fabricjs.com](http://fabricjs.com/) | Open source visual canvas libraries.                                 |
|                    | Dolby.io                                        | ❌        | $15–$50           | [dolby.io](https://dolby.io/)                | Paid API for audio enhancement, reverb, etc.                         |
| CI/CD              | GitHub Actions                                  | ✅        | $0                | [github.com/actions](https://github.com/features/actions) | Free for public; generous limits for private repos.                  |
| Monitoring         | LogRocket / Sentry                              | ✅        | $0–$25            | [logrocket.com](https://logrocket.com/), [sentry.io](https://sentry.io/) | Debugging & analytics tools with session replay.                     |

---

## 📊 Cost Summary Table

| Scenario               | Est. Monthly Total | Notes                                                       |
|------------------------|--------------------|-------------------------------------------------------------|
| Lean MVP (Free Tiers) | **$0–$20**         | Solo/small users, dev only, limited integrations            |
| Starter Growth         | **$50–$150**       | Paid Firebase, infra, and integration tiers                 |
| Scaled MVP             | **$150–$300+**     | Full-featured backend + paid audio, hosting, and services   |

---

## 🔮 Future Evolution (MVP-2+)

In future releases, this panel will be enhanced with:

- AI-powered moodboard suggestions  
- Contextual prompts based on file content  
- Generative remix prompts (e.g., "flip this like X artist")  
- Collaborative ideation (multi-user brainstorming with comments)  

---

## 🛣️ Roadmap

| MVP     | Focus                               | Timeline     |
|---------|--------------------------------------|--------------|
| MVP-1   | Brainstorming Skeleton (No AI)       | Q3 2025      |
| MVP-2   | AI/LLM features + Admin integrations | Q4 2025      |
| MVP-3+  | Production + ContentMarketing Flow   | 2026         |
