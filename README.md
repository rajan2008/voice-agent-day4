```md
```
# Day 4 – Teach-the-Tutor: Active Recall Coach  
### Murf AI Voice Agent Challenge (10 Days)

This project implements the **Day 4 Active Recall Tutor Voice Agent**, built using:

- **LiveKit Agents**
- **Murf Falcon TTS (Matthew, Alicia, Ken)**
- **Deepgram STT**
- **Google LLM**
- **Node.js frontend**

---

## 🎯 What This Agent Does

This day focuses on the **Teach-the-Tutor learning method**:

1. **Learn Mode**  
   The agent explains a concept using summaries from a JSON file.

2. **Quiz Mode**  
   The agent asks questions about that concept.

3. **Teach-Back Mode**  
   The agent asks the user to explain the concept back and gives feedback.

User can switch modes anytime by voice:

- “Switch to quiz mode”
- “Teach me loops”
- “Learn variables”
- “Go to teach back mode”

---

## 🧠 Powered by Content File

All concepts come from:
```
backend/shared-data/day4_tutor_content.json
```
yaml
Copy code

You can add more concepts easily.

---

## 🎤 Voices Used (Murf Falcon)

|    Mode    | Murf Voice |
|------------|------------|
| Learn      | Matthew    |
| Quiz       | Alicia     |
| Teach-Back | Ken        |

---

## ▶️ Run Backend
```
cd backend
python agent.py
```
yaml
Copy code

Backend starts the LiveKit agent.

---

## ▶️ Run Frontend

Frontend same as Day 1–3:
```
cd frontend
npm install
npm run dev
```
yaml
Copy code

Then open your browser to connect.

---

## 📝 Day 4 Deliverables

1. Working agent using all three modes  
2. Small JSON content file  
3. Screen recording showing all modes  
4. LinkedIn post tagging **@Murf AI**  
   - Use hashtags  
     - #MurfAIVoiceAgentsChallenge  
     - #10DaysofAIVoiceAgents  

---

## ✔ This completes Day 4.

# END OF README
