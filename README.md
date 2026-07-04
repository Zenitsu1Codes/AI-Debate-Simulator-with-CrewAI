# 🗣️ AI Debate Simulator with CrewAI

An AI-powered **Debate Simulator** built using **CrewAI** and **Groq Llama 3.3**. The system creates a structured debate where one AI agent argues **for** a motion, another argues **against** it, and a third AI judge evaluates both arguments to determine the winner.

This project demonstrates how multiple AI agents can collaborate to solve reasoning tasks through sequential workflows.

---

# ✨ Features

* 🤖 Multi-agent debate system
* 👍 AI generates arguments supporting a motion
* 👎 AI generates arguments opposing a motion
* ⚖️ Independent AI judge evaluates both sides
* 📝 Saves each stage of the debate as Markdown
* ⚡ Powered by Groq's Llama 3.3 70B model
* 📂 YAML-based agent and task configuration
* 🔄 Sequential CrewAI workflow

---

# 🛠 Tech Stack

* Python
* CrewAI
* Groq API
* Llama 3.3 70B Versatile
* YAML
* Python Dotenv

---

# 📂 Project Structure

```text
debate/
│
├── main.py
├── crew.py
├── requirements.txt
├── README.md
├── .env
│
├── config/
│   ├── agents.yaml
│   └── tasks.yaml
│
└── output/
    ├── propose.md
    ├── oppose.md
    └── decide.md
```

---

# 🧠 Architecture

```text
                    Motion
                      │
                      ▼
                Debate Crew
                      │
          ┌───────────┴───────────┐
          ▼                       ▼
   Propose Agent           Oppose Agent
          │                       │
          └───────────┬───────────┘
                      ▼
                Judge Agent
                      │
                      ▼
             Final Decision
```

---

# 🚀 Workflow

1. A debate motion is provided.
2. The **Debater Agent** argues in favor of the motion.
3. The **Debater Agent** argues against the same motion.
4. The **Judge Agent** reviews both arguments.
5. The final decision is saved as a Markdown report.

---

# ⚙️ Installation

Clone the repository.

```bash
git clone https://github.com/yourusername/ai-debate-simulator.git

cd ai-debate-simulator
```

Install dependencies.

```bash
pip install -r requirements.txt
```

---

# 🔑 Environment Variables

Create a `.env` file in the project root.

```env
GROQ_API_KEY=your_groq_api_key
OPENAI_API_KEY=your_openai_api_key
OPENAI_BASE_URL=https://api.groq.com/openai/v1
MODEL=llama-3.3-70b-versatile
```

---

# ▶️ Usage

Run the project:

```bash
python main.py
```

Example motion:

```python
inputs = {
    "motion": "There needs to be strict laws to regulate LLMs"
}
```

---

# 📄 Output

The project generates three Markdown files:

```text
output/
│
├── propose.md     # Arguments supporting the motion
├── oppose.md      # Arguments opposing the motion
└── decide.md      # Judge's final decision
```

---

# 💡 Example Motions

* Should AI replace software developers?
* Is remote work better than office work?
* Should social media be regulated?
* Should cryptocurrencies replace traditional banking?
* Is open-source AI safer than closed-source AI?
* Should autonomous vehicles become mandatory?
* Should governments regulate artificial intelligence?

---

# 📚 Learning Outcomes

This project demonstrates:

* Multi-Agent AI Systems
* CrewAI Framework
* Sequential Agent Workflows
* Prompt Engineering
* AI Reasoning
* Decision Making with LLMs
* YAML Configuration
* Automated Report Generation

---

# 🔮 Future Improvements

* Multiple debating rounds
* Rebuttal phase
* Audience voting
* Debate scoring system
* Debate history
* Streamlit or Gradio web interface
* Voice-based debates
* Multiple judges with majority voting
* PDF export of debate reports

---

# 👨‍💻 Author

**Harsh Asarsa**

AI • Python • CrewAI • Agentic AI • Multi-Agent Systems

If you found this project useful, consider giving it a ⭐ on GitHub.
