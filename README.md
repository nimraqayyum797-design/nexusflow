# ⚡ NexusFlow — The Next-Gen All-in-One Productivity & Knowledge Cockpit

> **Live Deployed Application:** [https://nexusflow-1.ai.studio/](https://nexusflow-1.ai.studio/)

---

## 📌 Executive Overview & Problem Statement

### What is NexusFlow?
**NexusFlow** is a high-performance, dark-mode personal operating system and productivity cockpit designed to synthesize daily task management, academic study workflows, habit streak building, spiritual (Islamic Barakah) alignment, personal journaling, and multi-persona AI assistance into a single, cohesive interface.

### The Real Problem Solved
High-performing creators, students, and professionals suffer from **app fragmentation**. Managing daily tasks in one app, tracking habits in another, studying with standalone flashcard tools, reflecting in a separate journal, and using generic chat bots for guidance leads to context switching, cognitive fatigue, and fractured focus.

### Who It Is For
- **Students & Lifelong Learners** who need structured study roadmaps, AI concept breakdowns, revision flashcards, and practice quizzes.
- **Productive Creators & Professionals** who require deep task decomposition, habit consistency tracking, and focus analytics.
- **Faith-Conscious Users** who want to harmonize material productivity with spiritual obligations (Salah routines, Quran goals, and daily Barakah tracking).

---

## 🖼️ Application Screenshots in Action

### 1. Unified Command Dashboard
![NexusFlow Command Dashboard](./src/assets/images/nexusflow_dashboard_preview_1785009037690.jpg)
*Interactive overview displaying habit completion rates, task velocity, study metrics, and quick action controls.*
<img width="1353" height="633" alt="dashboard png" src="https://github.com/user-attachments/assets/e43cf1c7-4b6b-4ae6-b118-0e9741ea0b1e" />
<img width="720" height="1459" alt="mobile png login page" src="https://github.com/user-attachments/assets/30444c89-1424-4eb4-9687-8f31f0778387" />

---

### 2. Multi-Persona AI Assistant
![NexusFlow AI Assistant Interface](./src/assets/images/nexusflow_ai_assistant_preview_1785009054507.jpg)
*Dedicated AI personas powered by Gemini 3.6 Flash providing tailored coaching, academic tutoring, focus exercises, and spiritual guidance.*
<img width="1355" height="638" alt="AI asistant workflow png" src="https://github.com/user-attachments/assets/02ea866e-5e90-4201-a54d-67cefac20c55" />


---

### 3. Academic Study Suite & Habit Matrix
![NexusFlow Study & Habit Engine](./src/assets/images/nexusflow_study_and_habits_preview_1785009073345.jpg)
*AI-generated revision flashcards, active quizzes, and weekly habit streak trackers.*
<img width="1344" height="645" alt="AI study hub workflow png" src="https://github.com/user-attachments/assets/0ac0ed9e-724c-4987-a1d9-6133b6a4b898" />

---

## ✨ Features & Capabilities

### 1. 📊 Interactive Command Dashboard
- **Real-Time Productivity Hub**: Monitor habit completion rates, pending tasks, study hours, and spiritual Barakah scores at a glance.
- **Quick Action Launcher**: 1-click modal triggers to log study sessions, add tasks, record habits, or log journal entries.
- **Top Header Profile Integration**: Clickable avatar in the top-left corner opens the user profile modal for identity management and theme customization.

### 2. 🧠 Multi-Persona AI Assistant
- **4 Specialised AI Personas**:
  - **AI Life Coach**: Goal setting, habit design, overcoming procrastination, and motivational routines.
  - **AI Study Tutor**: Academic breakdowns, exam roadmaps, and active recall coaching.
  - **AI Focus Assistant**: Tactical deep work sprint design, dopamine distraction blocking, and recovery advice.
  - **Islamic Productivity Companion**: Integrating faith obligations (Salah, Quran) with daily schedules for spiritual Barakah.

### 3. ✅ Smart Task Management with AI Breakdown
- **Energy & Priority Tagging**: Categorize tasks by difficulty, due date, and energy requirements (Low, Medium, High).
- **1-Click AI Subtask Generator**: Uses Gemini 3.6 Flash structured JSON output to automatically decompose complex tasks into 3–6 actionable micro-tasks with estimated completion times.

### 4. 📚 Academic Study Suite
- **AI Concept Explainer**: Get instant breakdowns of any topic using three modes:
  - *ELI5 (Explain Like I'm 10)* using intuitive analogies.
  - *Deep Academic Dive* with structured technical insights.
  - *3 Creative Real-World Analogies* for mental imagery.
- **AI Revision Flashcard Generator**: Input any subject to automatically generate 5 high-yield flashcards with interactive front/back flip animation.
- **AI Multiple-Choice Quiz Engine**: Instant 4-question quizzes with option choices, immediate grading, and explanation feedback.

### 5. 🔄 Habit & Streak Matrix
- **Custom Habit Tracking**: Track daily habits across categories (Health, Mind, Work, Faith).
- **Streak Counters & Frequency**: Visual weekly grid with interactive toggle checkboxes and percentage indicators.

### 6. 🌙 Islamic Barakah & Spiritual Hub
- **Salah Routine Log**: Track daily 5 prayers (Fajr, Dhuhr, Asr, Maghrib, Isha) with completion status.
- **Spiritual Metrics**: Log daily Quran recitation pages, Dhikr goals, and Islamic reflection notes.

### 7. 📈 Productivity Analytics & AI Auditing
- **Visual Charts**: Interactive Recharts analytics illustrating task completion velocity and weekly focus hour distribution.
- **AI Productivity Audit**: Analyzes current habits, task logs, and mood states to generate a 0–100 **Focus Score** along with strategic recommendations.

### 8. 📖 Interactive Personal Journal
- **Mood & Energy Logger**: Track daily emotional and cognitive energy levels.
- **Tagging & Search**: Categorize journal entries with custom tags and instant search filtering.

### 9. 🎨 Identity & Aesthetic Customization
- **Profile Modal**: Access user details, edit credentials, and switch workspace roles.
- **6 Dynamic Accent Themes**: Switch between Neon Lime (`#B6FF4D`), Cyan Spark (`#00D8F6`), Emerald (`#35D07F`), Classic Blue (`#0066FF`), Amber (`#F59E0B`), and Rose Glow (`#EC4899`).

---

## 🤖 AI Features, Models & System Prompts

NexusFlow is natively integrated with **Google Gemini 3.6 Flash** via the official `@google/genai` TypeScript SDK. All AI calls pass through secure server-side Express API proxies (`/api/gemini/*`) to ensure API key security.

### 1. Persona Chat System (`/api/gemini/chat`)
**Model**: `gemini-3.6-flash`

#### System Prompts by Persona:
- **AI Life Coach**:
  ```text
  You are the NexusFlow AI Life Coach. You are wise, motivating, empathetic, and highly strategic.
  Your goal is to help the user define high-impact personal goals, break down mental blocks, plan routines, overcome procrastination, and stay motivated.
  Provide extremely polished, actionable, and inspiring advice. Keep your tone sophisticated, calm, and encouraging. Use elegant formatting.
  ```
- **AI Study Tutor**:
  ```text
  You are the NexusFlow AI Study Tutor. You are exceptionally intelligent, clear-headed, and structured.
  Your goal is to explain complex academic, professional, or general concepts perfectly, create study schedules, and design custom learning roadmaps.
  Always break down concepts step-by-step. Use formatting, bold headers, and short bullet points to make things ultra-readable.
  ```
- **Islamic Companion**:
  ```text
  You are the NexusFlow Islamic Productivity Companion. You combine modern productivity principles with timeless Islamic wisdom.
  Your goal is to help the user balance spiritual obligations (like Salah, Quran, Dhikr) with daily studies, work, and wellness.
  Speak with deep respect, kindness, and wisdom. Suggest beautiful, practical ways to integrate faith into a busy lifestyle (e.g., using Barakah, focusing after Fajr, keeping consistent habits).
  ```
- **AI Focus Assistant**:
  ```text
  You are the NexusFlow AI Focus Assistant. You are tactical, crisp, and direct.
  Your goal is to help the user block out distractions, structure deep work sprints, manage cognitive energy levels, and enter deep flow states.
  Keep your answers brief, high-energy, and highly actionable. Give quick focus exercises, pomodoro structures, or immediate tips to get back to work.
  ```

---

### 2. AI Subtask Generator (`/api/gemini/subtasks`)
**Model**: `gemini-3.6-flash` (Structured Output Schema)
- **Prompt Instruction**:
  ```text
  Break down the task into a logical, step-by-step sequence of 3 to 6 micro-tasks (subtasks).
  Return the response STRICTLY as a JSON array where each object has "title" (string) and "estimatedMinutes" (number) properties.
  ```

---

### 3. AI Concept Explainer (`/api/gemini/study/explain`)
**Model**: `gemini-3.6-flash`
- **System Instruction**:
  ```text
  You are an elite Nobel Prize-winning teacher who explains complex concepts with perfect clarity, beautiful formatting, and inspiring tone.
  ```

---

### 4. AI Flashcard & Quiz Generators (`/api/gemini/study/flashcards`, `/api/gemini/study/quiz`)
**Model**: `gemini-3.6-flash` (Structured Output Schema)
- Generates high-yield study flashcards and 4-question multiple-choice quizzes with options, answer indices, and explanations enforcing JSON Schema validation.

---

### 5. AI Productivity Auditor (`/api/gemini/insights`)
**Model**: `gemini-3.6-flash` (Structured Output Schema)
- Evaluates habit logs, task completion metrics, and focus sprint records to return a calculated `focusScore`, `scoreJustification`, `productivityDiscovery`, `faithBalanceInsight`, and `immediateAction`.

---

## 🛠️ Tools, Services & Technologies Used

| Layer | Technology / Library | Purpose |
| :--- | :--- | :--- |
| **AI Model** | **Google Gemini 3.6 Flash** | Natural language reasoning, concept explanations, and structured JSON generation |
| **SDK** | `@google/genai` (v0.1.1) | Official Google Gen AI TypeScript SDK |
| **Frontend Framework** | **React 18** & **TypeScript** | Type-safe, component-driven user interface |
| **Build Tool** | **Vite** | Fast module bundling and dev environment |
| **Styling** | **Tailwind CSS v4** | Utility-first responsive dark theme styling |
| **Animations** | **Motion (`motion/react`)** | 60fps layout transitions, modal animations, and micro-interactions |
| **Icons** | **Lucide React** | Clean, minimalist visual icon system |
| **Data Visualization** | **Recharts** | Interactive graphs and productivity charts |
| **Backend Server** | **Node.js & Express.js** | Full-stack API routes for Gemini proxying and serving static assets |
| **Bundler (Backend)** | **esbuild** & **tsx** | Fast CommonJS server compilation into single output (`dist/server.cjs`) |
| **Environment** | **Google Cloud Run** | Containerized execution environment on port 3000 behind Nginx |

---

## 🚀 How to Run the Project Locally

### Prerequisites
- **Node.js** (v18 or higher)
- **npm** or **bun**
- A **Google Gemini API Key** (obtainable from [Google AI Studio](https://aistudio.google.com/))

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/nexusflow.git
cd nexusflow
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure Environment Variables
Create a `.env` file in the project root (reference `.env.example`):
```env
GEMINI_API_KEY=your_actual_gemini_api_key_here
PORT=3000
```

### 4. Start Development Mode
Run the full-stack server with Vite middleware integration:
```bash
npm run dev
```
Open your browser and navigate to `http://localhost:3000`.

### 5. Build for Production
To build both the React frontend and the bundled Express backend server:
```bash
npm run build
```

### 6. Start Production Server
Launch the compiled standalone CommonJS server:
```bash
npm start
```

---

## 📄 License & Credits

Built with precision for Google AI Studio. Designed and developed by **Nimra Qayyum**.
