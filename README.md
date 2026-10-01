# Career Conversation Agent Chatbot

> **Built by [Abdul Qudoos](https://www.abdul-qudoos.com)**, AI Automation & Forward Deployed Engineer · [More projects](https://www.abdul-qudoos.com/work)

A conversational AI chatbot that represents a professional (e.g., Abdul Qudoos) for career-related Q&A, built with Python, Gradio, Gemini (Google LLM), and Pushover notifications.

## Features
- Answers questions about the professional's background, skills, and experience using Gemini LLM.
- Reads summary and LinkedIn profile from PDF and text files.
- Sends push notifications via Pushover when a user provides their email or asks an unknown question.
- Simple web chat interface powered by Gradio.

## Agentic AI Capabilities
This chatbot is designed with agentic AI principles, enabling it to:
- **Autonomously use tools:** The agent can trigger internal functions (tools) such as recording user details or logging unknown questions, without user intervention.
- **Context-aware actions:** The agent maintains context from the user's conversation, using it to decide when to prompt for contact information or escalate unanswered questions.
- **Proactive engagement:** If the agent cannot answer a question, it records the event and can encourage the user to provide more information or get in touch.
- **Seamless integration:** Tool use and notifications are handled in the background, so the user experience remains natural and uninterrupted.
- **Extendable agent framework:** The architecture allows for easy addition of new tools or actions, making the agent adaptable to new requirements or workflows.

## Setup

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/Career_Conversation_agent_Chatbot.git
cd Career_Conversation_agent_Chatbot
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Prepare required files
- Place your LinkedIn PDF and summary text in the `me/` directory:
  - `me/YourCV.pdf` (or update the filename in `app.py`)
  - `me/summary.txt`

### 4. Set up environment variables
Create a `.env` file in the project root with the following:
```
GEMINI_API_KEY=your_gemini_api_key
PUSHOVER_TOKEN=your_pushover_app_token
PUSHOVER_USER=your_pushover_user_key
```

### 5. Run the app
```bash
python app.py
```
- Open the local URL shown in the terminal (e.g., http://127.0.0.1:7860/) in your browser.

## Notifications
- When a user provides their email or asks a question the bot can't answer, a push notification is sent to your Pushover app.
- Make sure you have the Pushover app installed and are logged in with the correct user key.

## Customization
- To change the represented professional, update the name, PDF, and summary in `app.py` and the `me/` directory.
- To use a different LLM, adapt the `chat` method in `app.py`.

---

## About the author

I'm **Abdul Qudoos**, an AI automation and forward deployed engineer based in Islamabad, Pakistan. I build production AI agents, voice agents, workflow automation, and the full-stack products around them.

- Portfolio: [abdul-qudoos.com](https://www.abdul-qudoos.com)
- Case studies: [abdul-qudoos.com/work](https://www.abdul-qudoos.com/work)
- LinkedIn: [Abdul Qudoos](https://www.linkedin.com/in/abdul-qudoos-9a4640324/)
- Email: abdulqudoos7113@gmail.com
