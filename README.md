# MELODI

<aside>
🖥️

## Tech Stack

</aside>

### **Overview**

Our SaaS platform empowers independent musicians by offering a project management tool tailored for creative workflows. It includes high quality databasing tools, media-rich integrations (Spotify, Pinterest), audio processing, and a visual canvas for moodboarding and asset organization.

---

### **Frontend**

- **Framework**: React (with React Native for mobile support)
    
    <aside>
    🛠 Front-end development tool; Code in Javascript
    
    </aside>
    
- **Drag-and-Drop UI**: `react-beautiful-dnd` for intuitive, card-based interface
    
    <aside>
    🛠 UI Builder for React
    
    </aside>
    
- **Real-Time Collaboration**: WebSockets or Firebase for updates (chat, edits)
    
    <aside>
    🛠 Tracks real-time updates for user-made edits
    
    </aside>
    
- **Visual Canvas**: Custom-built drag-and-drop grid canvas inspired by Milanote
    - Libraries: `Konva.js` or `fabric.js` for 2D canvas rendering and manipulation
        
        <aside>
        🛠 Creating visual canvases, similar to Figma or Milanote
        
        </aside>
        
- **Audio Player UI**: Waveform visualization via `wavesurfer.js` or `howler.js`
    
    <aside>
    🛠 Displays waveform; more just for visuals
    
    </aside>
    

---

### **Backend**

- **API Development**: Node.js (Express) or Python (FastAPI)
    
    <aside>
    🛠 Backend language
    
    </aside>
    
- **Database**:
    - PostgreSQL for relational data (projects, users, notes)
    
    <aside>
    🛠 Structured database; rows and columns; typically for text, memos, and sheets
    
    </aside>
    
    - MongoDB for unstructured content (media uploads, canvas objects)
    
    <aside>
    🛠 Unstructured database; for free-form content like media
    
    </aside>
    
- **Authentication & Realtime Backend**: Firebase Auth + Firebase Firestore or Supabase as alternative
    
    <aside>
    🛠 User authentication
    
    </aside>
    
- **Audio Processing API**:
    - Server-side rendering of audio (Reverb, EQ, Compression)
    - Tools: `ffmpeg`, `sox`, or Node.js-based audio libraries like `audiomass`, `Tone.js`
        
        <aside>
        🛠 Renders audio for processing
        
        </aside>
        

---

### **Third-Party Integrations Via Zapier or Make.com:**

<aside>
🛠 Automation/Integration between our platform to third-party software

</aside>

- **Pinterest**: Pull inspiration images or feeds into user boards
- **Spotify**:
    - Import related artists data
    - Fetch track/playlist metadata
    - Embed Spotify players in canvas or notes

---

### **File Management & Media**

- **Cloud Storage**: Firebase Storage or AWS S3 for audio/image files
    
    <aside>
    🛠 Storage for all assets
    
    </aside>
    
- **Transcoding**: Server-side `ffmpeg` or integration with services like Dolby.io for high-quality audio processing
    
    <aside>
    ⚠️
    
    SAVE FOR FUTURE DATE: Audio transcoding for higher quality files; will probably be out of our scope
    
    </aside>
    

---

### **Infrastructure & DevOps**

- **Hosting**: Vercel for frontend, Render or Heroku for backend (starter-friendly)
    
    <aside>
    🛠 Vercel used to build the web platform; Render or Heroku for Backend
    
    </aside>
    
- **CI/CD**: GitHub Actions
    
    <aside>
    🛠 Git actions to navigate 
    
    </aside>
    
- **Monitoring**: LogRocket (frontend), Sentry (backend)
    
    <aside>
    ⚠️ SAVE FOR FUTURE DATE: Essentially a CRM tool for frontend and backend updates and debugging
    
    </aside>
    

---

### **Planned MVP Features**

| Feature | Stack / Tooling |
| --- | --- |
| Drag-and-drop interface | React + `react-beautiful-dnd` |
| Real-time updates | WebSockets / Firebase |
| Pinterest integration | Zapier/Make → Pinterest API |
| Spotify integration | Zapier/Make → Spotify API |
| Audio editing | `ffmpeg`, `Tone.js`, or `Web Audio API` |
| Canvas/Moodboard | `Konva.js`, `fabric.js`, or `react-flow` |
| Authentication | Firebase Auth |
| Database | PostgreSQL (structured) + MongoDB (unstructured) |

---

### 💼 **Tech Stack with Costs, Links, and Notes**

| **Category** | **Service/Tool** | **Free Tier?** | **Est. Monthly Cost** | **Link** | **Notes** |
| --- | --- | --- | --- | --- | --- |
| **Frontend Hosting** | [Vercel](https://vercel.com/pricing) | ✅ | $0–$20 | [vercel.com](https://vercel.com/) | Free for hobby/dev. Pro plan ($20/mo) adds analytics and team features. |
| **Backend Hosting** | [Render](https://render.com/pricing) / [Railway](https://railway.app/pricing) | ✅ | $7–$25 | [render.com](https://render.com/) / [railway.app](https://railway.app/) | Affordable server hosting. Free tier with limits; paid plans start from $7–$15. |
| **Database** | [Supabase (PostgreSQL)](https://supabase.com/pricing) | ✅ | $0–$25 | [supabase.com](https://supabase.com/) | Free up to 500MB; paid plans include more performance and backups. |
|  | [MongoDB Atlas](https://www.mongodb.com/atlas/database/pricing) | ✅ | $0–$30 | [mongodb.com](https://www.mongodb.com/atlas) | M0 free tier for dev. Storage & usage costs rise quickly in production. |
| **Auth** | [Firebase Auth](https://firebase.google.com/pricing) | ✅ | $0–$20 | [firebase.google.com](https://firebase.google.com/) | Free up to 10K monthly verifications. Paid plans based on auth volume. |
| **Storage** | [Firebase Storage](https://firebase.google.com/pricing) / [AWS S3](https://aws.amazon.com/s3/pricing/) | ✅ | $5–$20 | [firebase.google.com](https://firebase.google.com/) / [aws.amazon.com](https://aws.amazon.com/s3) | Firebase good for smaller media use. S3 better at scale. Pricing varies by region and usage. |
| **Realtime Backend** | [Firebase Firestore](https://firebase.google.com/pricing) | ✅ | $0–$25 | [firebase.google.com](https://firebase.google.com/) | Free up to 50K reads/day. Careful with aggressive real-time sync. |
| **Integrations** | [Zapier](https://zapier.com/pricing) | ✅ | $0–$19 | [zapier.com](https://zapier.com/) | Free tier has 100 tasks/month. Starter plan gives multi-step zaps. |
|  | [Make.com](https://www.make.com/en/pricing) | ✅ | $0–$16 | [make.com](https://www.make.com/) | Free for 1,000 ops/mo. Basic plan expands task capacity and support. |
| **Audio Processing** | [FFmpeg](https://ffmpeg.org/) / [Sox](http://sox.sourceforge.net/) | ✅ | $0 (infra only) | [ffmpeg.org](https://ffmpeg.org/) / [sox.sourceforge.net](http://sox.sourceforge.net/) | Open source tools. Costs only relate to server compute time. |
| **Canvas/Visuals** | [Konva.js](https://konvajs.org/) / [Fabric.js](http://fabricjs.com/) | ✅ | $0 | [konvajs.org](https://konvajs.org/) / [fabricjs.com](http://fabricjs.com/) | Open source canvas rendering libs. No direct cost. |
|  | [Dolby.io](https://dolby.io/communications/pricing/) | ❌ | $15–$50 | [dolby.io](https://dolby.io/) | Pay-as-you-go for audio APIs (enhancement, reverb, noise reduction). |
| **CI/CD** | [GitHub Actions](https://github.com/features/actions) | ✅ | $0 | [github.com/actions](https://github.com/features/actions) | Free for public repos; generous limits for private ones too. |
| **Monitoring** | [LogRocket](https://logrocket.com/pricing) / [Sentry](https://sentry.io/pricing/) | ✅ | $0–$25 | [logrocket.com](https://logrocket.com/) / [sentry.io](https://sentry.io/) | Great for bug reporting & session replay. Free tiers available. |

---

### 📊 **Cost Summary Table**

| **Scenario** | **Est. Monthly Total** | **Notes** |
| --- | --- | --- |
| Lean MVP (Free Tiers) | **$0–$20** | For solo/few users, dev only, limited integrations |
| Starter Growth | **$50–$150** | Paid plans for Firebase, hosting, and basic integrations |
| Scaled MVP (All Paid Plans) | **$150–$300+** | Includes audio API, upgraded Zapier, better infra & storage |

---

### 🔮 Future Evolution (MVP-2+)

In future releases, this panel will be enhanced with:

- AI-powered moodboard suggestions
- Contextual prompts based on file content
- Generative remix prompts (e.g., "flip this like X artist")
- Collaborative ideation (multi-user brainstorming with comments)

---

### **🛣️ Roadmap**

| **MVP** | **Focus** | **Timeline** |
| --- | --- | --- |
| MVP-1 | Brainstorming Skeleton (No AI) | Now (Target Q3 2025) |
| MVP-2 | AI/LLM features + Admin integrations | Q4 2025 |
| MVP-3+ | Production + ContentMarketing Workflows | 2026 |
