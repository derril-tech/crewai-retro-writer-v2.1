# 🔄 CrewAI RetroWriter
**Powered by CrewAI + OpenAI**


> **Transform sprint chaos into actionable insights. Connect your Jira or Linear workspace, and let 6 AI agents generate a facilitator-ready retrospective in seconds.** ⚡

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.11+-blue.svg)](https://www.python.org/downloads/)
[![Next.js](https://img.shields.io/badge/Next.js-15-black.svg)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-19-61DAFB.svg)](https://react.dev/)
[![CrewAI](https://img.shields.io/badge/CrewAI-Multi_Agent-purple.svg)](https://www.crewai.com/)
[![Railway](https://img.shields.io/badge/Deploy-Railway-blueviolet.svg)](https://railway.app/)

---

## ✨ What It Does

RetroWriter is an intelligent retrospective automation platform that orchestrates **6 specialized CrewAI agents** to:

1. **📊 Collect Sprint Data** — Pull issues, comments, and metadata from Jira or Linear
2. **🔍 Analyze Themes** — Identify patterns, root causes, and recurring issues
3. **✅ Extract Wins** — Celebrate achievements and successful deliveries
4. **⚠️ Surface Challenges** — Document blockers with constructive insights
5. **💡 Capture Learnings** — Extract knowledge and insights gained
6. **📋 Generate Action Items** — Create SMART items with owners and due dates

All orchestrated through a beautiful interface with real-time progress tracking.

---

## 🎯 Core Features

### 🤖 **Multi-Agent AI System**
- **6 Specialized Agents** — Each with distinct expertise and responsibilities
- **CrewAI Orchestration** — Agents collaborate to produce comprehensive retros
- **OpenAI GPT-4.1** — Intelligent analysis powered by latest models
- **Real-time Progress** — Watch agents work with live activity stream

### 🔗 **Native Integrations**
- **Jira Cloud** — Connect boards, sprints, and issues via REST API
- **Linear** — Teams, cycles, and issues with GraphQL API
- **Automatic Caching** — 5-minute cache reduces API calls
- **Fallback Support** — Works with mock data when APIs unavailable

### 📄 **Structured Output**
- **What Went Well** — Achievements, wins, and successes
- **What Didn't Go Well** — Blockers, delays, and challenges
- **Learnings** — Team insights and knowledge gained
- **Action Items** — SMART goals with owners and due dates

### 🎨 **Modern UI/UX**
- **Dark/Light Mode** — Beautiful themes with system preference support
- **Mobile-First** — Responsive design with 44px+ touch targets
- **Real-time Updates** — Live job status and agent activity
- **Export Options** — Markdown, JSON, HTML, and plain text

### 📱 **Full Feature Set**
| Feature | Description |
|---------|-------------|
| 🔄 **Sprint Selection** | Choose boards/teams and sprints/cycles |
| 👀 **Live Agent View** | Watch 6 agents process your data |
| ✏️ **Inline Editing** | Edit any section before sharing |
| 📊 **Summary Dashboard** | Visual stats and insights |
| 📋 **Action Item Manager** | Drag, edit, prioritize items |
| 📁 **Export Options** | MD, JSON, HTML, TXT formats |
| 💬 **AI Chat Coach** | Ask follow-up questions |
| 📜 **Retro History** | View and compare past retros |
| 🎯 **Interactive Tour** | Onboarding for new users |
| ⌨️ **Keyboard Shortcuts** | Power user navigation |
| 🖨️ **Print Ready** | Professional print formatting |
| 📧 **Email Share** | Send retros via email |

---

## 🏗️ Tech Stack

### **Frontend** ⚛️
| Technology | Purpose |
|------------|---------|
| **Next.js 15** | React 19 with App Router |
| **TypeScript** | Type-safe development |
| **Tailwind CSS** | Utility-first styling |
| **shadcn/ui** | Beautiful component library |
| **Lucide Icons** | Modern icon set |

### **Backend** 🐍
| Technology | Purpose |
|------------|---------|
| **FastAPI** | High-performance Python API |
| **CrewAI** | Multi-agent AI orchestration |
| **OpenAI GPT-4.1** | Intelligent text generation |
| **Pydantic v2** | Data validation |

### **Data & Cache** 💾
| Technology | Purpose |
|------------|---------|
| **Supabase** | PostgreSQL persistence |
| **Upstash Redis** | Job queue & caching |

### **External APIs** 🔌
| API | Purpose |
|-----|---------|
| **Jira Cloud** | Sprint and issue data |
| **Linear** | Cycle and issue data |
| **OpenAI** | GPT-4.1-mini for analysis |

### **Deployment** 🚀
| Platform | Service |
|----------|---------|
| **Vercel** | Frontend hosting |
| **Railway** | Backend API |

---

## 🔄 How It Works

```
┌─────────────────────────────────────────────────────────────┐
│                    USER INPUT                               │
│           Select Board/Team + Sprint/Cycle                  │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│              JIRA / LINEAR API FETCH                        │
│         Issues, Comments, Metadata, Assignees               │
└─────────────────────┬───────────────────────────────────────┘
                      │
                      ▼
┌─────────────────────────────────────────────────────────────┐
│                  CREWAI WORKFLOW                            │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────┐      │
│  │    Data      │  │   Theme      │  │  Positives   │      │
│  │  Collector   │──│  Analyzer    │──│   Agent      │      │
│  └──────────────┘  └──────────────┘  └──────┬───────┘      │
│                                             │               │
│  ┌──────────────┐  ┌──────────────┐  ┌──────▼───────┐      │
│  │  Negatives   │──│   Action     │──│ Facilitator  │      │
│  │    Agent     │  │ Item Agent   │  │   Writer     │      │
│  └──────────────┘  └──────────────┘  └──────────────┘      │
└─────────────────────────────────────────────┬───────────────┘
                                              │
                                              ▼
┌─────────────────────────────────────────────────────────────┐
│                       OUTPUT                                │
│  • What Went Well (achievements, wins)                      │
│  • What Didn't Go Well (blockers, challenges)               │
│  • Learnings (insights, knowledge)                          │
│  • Action Items (SMART goals with owners)                   │
└─────────────────────────────────────────────────────────────┘
```

---

## 🎨 Customization

### Theme Options
- ☀️ **Light Mode** — Clean, professional interface
- 🌙 **Dark Mode** — Easy on the eyes
- 🖥️ **System** — Follows OS preference

### Export Formats
- 📝 **Markdown** — Perfect for wikis and docs
- 📋 **JSON** — For integrations and automation
- 🌐 **HTML** — Standalone web page
- 📄 **Plain Text** — Universal compatibility

---

## 📊 Performance

| Metric | Value |
|--------|-------|
| Retro Generation | ~15-30 seconds |
| Agent Count | 6 specialized agents |
| Mobile Ready | ✅ Yes |
| Offline Fallback | ✅ Mock data support |

---

## 🛡️ Security

- ✅ No sprint data stored permanently (processed ephemerally)
- ✅ API rate limiting and caching
- ✅ CORS protection for API endpoints
- ✅ Environment variables for all secrets
- ✅ Input validation with Pydantic

---

## 👨‍💻 Creator

**Derril Filemon**

This project demonstrates proficiency in:
- 🤖 **AI/ML Integration** — CrewAI multi-agent workflows, OpenAI GPT-4.1
- ⚛️ **Modern React** — Next.js 15, React 19, App Router, TypeScript
- 🐍 **Python Backend** — FastAPI, async/await, Pydantic v2
- 🎨 **UI/UX Design** — Responsive design, dark mode, accessibility
- ☁️ **Cloud Architecture** — Supabase, Redis, Railway, Vercel
- 🔗 **API Integrations** — Jira Cloud, Linear, OpenAI

---

## 🙏 Acknowledgments

- **[CrewAI](https://www.crewai.com/)** — Multi-agent orchestration framework
- **[OpenAI](https://openai.com/)** — GPT-4.1 API
- **[Supabase](https://supabase.com/)** — Database & auth
- **[Upstash](https://upstash.com/)** — Redis caching
- **[Railway](https://railway.app/)** — Backend deployment
- **[Vercel](https://vercel.com/)** — Frontend hosting
- **[shadcn/ui](https://ui.shadcn.com/)** — Beautiful components
- **[Atlassian](https://www.atlassian.com/)** — Jira Cloud API
- **[Linear](https://linear.app/)** — Linear API

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

**⭐ Star this repo if you find it useful!**

Made with ❤️ and ☕ by [Derril Filemon](https://github.com/derril-tech)

</div>
