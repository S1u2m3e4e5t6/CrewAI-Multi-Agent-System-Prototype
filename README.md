## 🤖 CrewAI Multi-Agent System Prototype
This project is a crash course and demonstration of a CrewAI-based multi-agent system. It showcases how to orchestrate autonomous AI agents to collaborate on complex tasks, such as market research and content creation.

The system is designed with a clear, extensible architecture, allowing you to easily define new agents, assign unique tasks, and build powerful, collaborative AI workflows.

---

## 🧠 Core Concept: The Research Crew
To demonstrate the framework, this prototype implements a "Market Research Crew" designed to analyze a topic and generate a report.

The Crew consists of two agents:

Market Researcher (researcher): This agent is responsible for Browse the web to find and gather relevant, up-to-date information on a given topic.

Content Strategist (writer): This agent takes the raw data from the researcher, identifies key insights, and structures them into a coherent and well-written report.

The Workflow:

The Researcher is tasked with finding the latest trends in AI.

It passes its findings to the Content Strategist.

The Strategist synthesizes the information and writes a final blog post.

The process is orchestrated by CrewAI, ensuring seamless task delegation and execution.
---

## 🚀 Features
Multi-Agent Orchestration: Multiple autonomous agents working together in a coordinated crew.

Dynamic Task Delegation: Agents can assign and receive tasks based on their defined roles and capabilities.

Sequential Workflows: Define clear, step-by-step processes for your agents to follow.

Configurable Agents: Easily define unique roles, backstories, and tools for each agent.

Extensible Architecture: Add new agents or modify workflows with minimal code changes.
---

## 🛠️ Tech Stack
Core Language: Python

AI Framework: CrewAI & LangChain for multi-agent orchestration.

LLM Provider: OpenAI for natural language understanding and generation.

UI (Optional): Streamlit for building an interactive front-end to monitor the agents.
---
## ⚙️ Setup and Installation
Follow these steps to get the project running on your local machine.

1. Clone the Repository
git clone https://github.com/yourusername/crewai-multi-agent-prototype.git
cd crewai-multi-agent-prototype
2. Install Dependencies
Install the required Python packages using pip.
pip install -r requirements.txt
3. Configure API Keys
For the agents to function, they need access to the OpenAI API.

Create a file named .env in the root directory of the project.

Add your OpenAI API key to the file like this:
OPENAI_API_KEY="sk-YourSecretAPIKeyHere"

## ▶️ Usage
Run the main script from the terminal to start the agent crew.
python main.py
You will see the agents collaborating in real-time in your terminal, printing their actions, and passing information to one another until the final report is generated.

## 📂 Project Structure
```
.
├── agents/            # Agent definitions (e.g., researcher, writer)
├── workflows/         # Task definitions and crew orchestration
├── utils/             # Helper functions and utilities
├── main.py            # Main script to run the crew
├── requirements.txt   # Project dependencies
└── .env               # For storing API keys (not committed to Git)
```
