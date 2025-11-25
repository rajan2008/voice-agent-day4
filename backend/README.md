# 📘 BACKEND README (backend/README.md)
✔ correct install
✔ correct requirements
✔ correct file structure
✔ no broken packages
✔ LiveKit + Murf usage
✔ working instructions
backend/README.md
# Day 4 – Teach-the-Tutor Active Recall Coach (Backend)

This folder contains the backend for **Day 4 of the Murf AI Voice Agent Challenge**.

It runs a LiveKit Voice Agent with 3 learning modes:
- **Learn** → explains a concept (Murf Voice: Matthew)
- **Quiz** → asks questions (Murf Voice: Alicia)
- **Teach-Back** → asks user to explain concept back (Murf Voice: Ken)

The agent loads a small course file (`day4_tutor_content.json`) and switches between modes anytime the user asks.

---

## 📁 Folder Structure



backend/
│
├── agent.py
├── requirements.txt
├── .env.local
├── shared-data/
│ └── day4_tutor_content.json
└── README.md (this file)


---

## 🔑 Environment Variables (`.env.local`)

Create a `.env.local` file inside backend with:



LIVEKIT_URL=ws://localhost:7880
LIVEKIT_API_KEY=devkey
LIVEKIT_API_SECRET=secret
MURF_API_KEY=your_murf_api_key
DEEPGRAM_API_KEY=your_deepgram_key
GOOGLE_APPLICATION_CREDENTIALS=your_google_json_path


---

## 📦 Install Dependencies

Activate virtual environment:

### Windows:
```sh
.\.venv\Scripts\activate

Install required packages:
pip install -r requirements.txt
```
📦 requirements.txt

Use exactly this:
```
livekit-agents
livekit-plugins-deepgram
livekit-plugins-google
livekit-plugins-silero
python-dotenv

```
💡 Note:
There is no package called livekit-plugins-murf or livekit-plugins-turn-detection.
The Murf plugin is included already inside livekit-agents.

▶️ Run Backend

Inside /backend:
```
python agent.py
```

You should see:

DAY 4 ACTIVE RECALL TUTOR LOADED
DAY 4 TUTOR AGENT STARTING

🎧 Voice Agent Modes

The agent chooses Murf voices automatically:

Mode	Voice
learn	Matthew
quiz	Alicia
teach_back	Ken
📚 Content File (shared-data/day4_tutor_content.json)
```
[
  {
    "id": "variables",
    "title": "Variables",
    "summary": "Variables store data values that your program can use or modify later.",
    "sample_question": "What is a variable and why do we use it?"
  },
  {
    "id": "loops",
    "title": "Loops",
    "summary": "Loops repeat a block of code multiple times so the program can perform repetitive tasks efficiently.",
    "sample_question": "Explain the difference between a for loop and a while loop."
  }
]
```
✔ You are ready to run the backend.
```
python agent.py
```
