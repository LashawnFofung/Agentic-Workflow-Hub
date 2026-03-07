# 🧪 Lab 01: The Autonomous Research Agent

## My First Agent

**Tool-Use**
The Research Agent 

----

## Building The AI Agent


**n8n Prompt**

Create an AI Agent workflow using the AI Agent node. It should start with a Chat Trigger. The agent needs to be connected to Google Gemini as the model, Window Buffer Memory for context, and a Google Search (SerpApi) tool. The goal is for the agent to research any topic I provide and return a structured report.

<br>

**In-action**
The agent will search the web, analyze the information, and return a comprehensive structured report with all the key details organized into clear sections.
Let me know if you'd like to adjust the report structure, add more tools, or modify how the agent behaves!

<br>

**Connection Port	What to connect it to	Purpose**

- <b>Chat Trigger:</b>	This is the "Data flow"—the user's message enters here.

- <b>AI Language Model - Google Gemini Chat Model:</b>	This is the "Brain"—the agent's reasoning engine.

- <b>AI Memory - Window Buffer Memory:</b>	This is the "Memory"—what the agent remembers from 5 minutes ago.

- <b>AI Tool - SerpApi (Google Search):	These are the "Hands"—the tools the agent can use to perform actions.

