# 🤖 Agentic AI Workflows: n8n & Gemini Labs

Welcome to my Agentic AI Laboratory. This repository serves as a professional portfolio and a technical sandbox for building autonomous systems using **n8n** and **Google Gemini (LLMs)**.

The goal of these labs is to move beyond simple "linear" automation and into **Agentic Workflows**—where the AI has "tools" (Search, Database, Email) and the reasoning power to decide how to use them to solve complex tasks.

---

## 🛠️ Tech Stack
* **Orchestrator:** [n8n](https://n8n.io/) (Low-code workflow automation)
* **Brain:** Google Gemini 1.5 Flash / 2.0 (via Google AI Studio)
* **Memory:** Window Buffer Memory
* **Tools:** Brave Search API / SerpApi / Custom HTTP Tools

---

## 🧪 Lab 01: The Autonomous Research Agent
This is my foundational project demonstrating the **"Agentic Loop."**

<b>🚀 Quick Start Guide: Lab 01</b>
  
  To get this agent running, you need to connect its "Brain" and its "Hands." Follow these steps:

   <b>1. 🧠 Connect the Brain (Google Gemini)</b>

  - <b>1. Get your Key:</b> Go to Google AI Studio and click "Create API key".
  
  - <b>2. Add to n8n:</b> Open the Google Gemini Chat Model node.
  
    - Under "Credential for Google Gemini API," click Create New Credential.
    
    - Paste your key and click Save.
  
  - <b>3. Select Model:</b> Ensure the Model field is set to gemini-1.5-flash or gemini-2.0-flash.

<b>2. 🔍 Connect the Hands (Search Tool)</b>

  - <b>1. Get your Key:</b> Go to SerpApi.com and create a free account. Copy your API Key from the dashboard.
  
  - <b>2. Add to n8n:</b>
  
    - Open the [SerpApi](https://serpapi.com/) node.
    
    - Under "Credential for SerpApi," click Create New Credential.
    
    - Paste your key and click Save.

<b>3. 🏁 Run Your First Test</b>

  - <b>1. Click the "Chat" button at the bottom of the n8n canvas.
  
  - <b>2. Type a request like:</b> "Research the top 3 AI automation trends for 2026."
  
  - <b>3. Observe the "Thought Process":</b> You will see the AI Agent node light up, call the search tool, and then generate your report.
     
### 🎯 Objective
Create an agent capable of performing live web research to bypass LLM knowledge cutoffs and provide structured, up-to-date reports.

### 🧩 Logic Flow
1. **User Input:** Receives a research topic via Chat Trigger.
2. **Reasoning:** Gemini LLM analyzes the request and determines if it needs "live" data.
3. **Tool Use:** The Agent calls the **Search Tool** to browse the web.
4. **Synthesis:** Gemini processes the search results and formats them into a professional report.

### 📥 How to Use
1. Install [n8n](https://docs.n8n.io/hosting/installation/).
2. Import the `research-agent.json` file located in the `/Labs/01-research-agent` folder.
3. Add your **Google Gemini API Key** and **Search API Key** to the credentials.
4. Open the Chat window and start researching!

---

## 📈 Future Labs (In Development)
- [ ] **Lead Enrichment Agent:** Automated LinkedIn/Web scraping for sales ops.
- [ ] **Email Triage Agent:** Categorizing and drafting replies based on sentiment.
- [ ] **Multi-Agent Debate:** Two agents debating a topic to find the best solution.

---

## 📄 License
This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.
