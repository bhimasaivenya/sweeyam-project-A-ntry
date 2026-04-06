# 🚀 A-ntry

## Agentic AI for Autonomous Business Decision-Making

A hackathon-ready demo showcasing how AI agents can autonomously monitor business metrics, detect anomalies, reason about root causes, and recommend actions—with human approval.

---

## ✨ Features

- **Multi-Agent System**: Observer, Analyst, Simulator & Decision agents
- **Gemini LLM Integration**: Powered by Google's Gemini 1.5 Flash
- **Real-time Dashboard**: Live metrics with beautiful charts
- **Keyboard Shortcuts**: Space to trigger, R to reset, A to approve
- **Sound Notifications**: Audio feedback for events
- **Confetti Celebration**: Visual reward on approval
- **Dark/Light Theme**: Toggle between themes
- **Human Governance**: Approve, modify, or reject AI recommendations

---

## 🚀 Quick Start

### 1. Install Dependencies

```bash
cd autopilot-ai/backend
pip install -r requirements.txt
```

### 2. Run the Server

```bash
python main.py
```

### 3. Open Browser

Navigate to: **http://localhost:8000**

---

## 🎮 How to Demo

1. **Observe** the healthy dashboard (green metrics, smooth charts)
2. **Press SPACE** or click the red button to simulate a crash
3. **Watch** the agent pipeline execute:
   - Observer detects anomaly
   - Analyst explains root cause (Gemini)
   - Simulator evaluates options
   - Decision Agent recommends action
4. **Review** the recommendation with confidence score
5. **Press A** or click Approve to confirm
6. **Enjoy** the confetti! 🎉

---

## 🔑 Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Space` | Trigger crash simulation |
| `R` | Reset system |
| `A` | Approve recommendation |
| `Esc` | Close modal |

---

## 🏗️ Architecture

```
┌─────────────────────────────────────────┐
│              FRONTEND                    │
│  Dashboard → Crash Button → Approval    │
└─────────────────────────────────────────┘
                    │
                    ▼
┌─────────────────────────────────────────┐
│           AGENT PIPELINE                 │
│                                          │
│  Observer → Analyst → Simulator → Decide │
│  (Rules)    (Gemini)   (Rules+   (Gemini)│
│                        Gemini)           │
└─────────────────────────────────────────┘
                    │
                    ▼
┌─────────────────────────────────────────┐
│         HUMAN GOVERNANCE                 │
│     Approve │ Modify │ Reject           │
└─────────────────────────────────────────┘
```

---

## 📁 Project Structure

```
autopilot-ai/
├── backend/
│   ├── agents/
│   │   ├── observer.py   # Rule-based detection
│   │   ├── analyst.py    # Gemini reasoning
│   │   ├── simulator.py  # Action simulation
│   │   └── decision.py   # Final recommendation
│   ├── data_generator.py # Synthetic e-commerce data
│   ├── main.py           # FastAPI server
│   └── requirements.txt
├── frontend/
│   ├── index.html
│   ├── styles.css
│   └── app.js
├── .env                   # Gemini API key
└── README.md
```

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/metrics` | 24h of business metrics |
| GET | `/api/kpis` | Current KPIs |
| POST | `/api/crash` | Trigger crash simulation |
| POST | `/api/reset` | Reset to healthy state |
| GET | `/api/agents/messages` | Agent activity log |
| POST | `/api/approve` | Process human approval |

---

## 📌 Why This is Special

### Agentic AI
- **Autonomous**: Agents work without human prompting
- **Specialized**: Each agent has a specific role
- **Collaborative**: Agents pass context to each other
- **Accountable**: Human must approve before execution

### LLM Usage
| Agent | LLM? | Purpose |
|-------|------|---------|
| Observer | ❌ | Rule-based detection |
| Analyst | ✅ | Root cause reasoning |
| Simulator | ✅ | Action explanations |
| Decision | ✅ | Final recommendation |

### Unique Features
- Keyboard shortcuts for fast demos
- Sound effects for engagement
- Confetti celebration
- Minimal, modern UI
- Real-time pipeline visualization

---

## 🎯 Demo Tips

1. Start with healthy metrics visible
2. Build tension before the crash
3. Narrate each agent's output
4. Highlight the confidence score
5. Ask audience: "Would you trust this AI?"
6. Show the human governance step
7. Celebrate with confetti!

---

**Built for hackathons with ❤️**
