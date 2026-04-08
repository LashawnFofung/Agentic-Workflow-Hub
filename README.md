# 🤖 Agentic AI Workflows: n8n & Gemini Labs

Welcome to my Agentic AI Laboratory. This repository serves as a professional portfolio and a technical sandbox for building autonomous systems using **n8n** and **Google Gemini (LLMs)**.

The goal of these labs is to move beyond simple "linear" automation and into **Agentic Workflows**—where the AI has "tools" (Search, Database, Email) and the reasoning power to decide how to use them to solve complex tasks.

---

## 🛠️ Tech Stack
* **Orchestrator:** [n8n](https://n8n.io/) (Low-code workflow automation)
* **Brain:** Google Gemini 1.5 Flash / 2.0 (via Google AI Studio) 
* **Memory:**
  - **Logging Node:** Stores "Generation Metadata," such as the number of products analyzed and the "Trend Confidence Score" for each run.
  - **Wait Node:** Used to ensure data from previous steps is fully processed before moving to the next stage of the workflow.
  - **Merge/Code Nodes:** Act as temporary working memory to combine and structure information from different data sources (e.g., Amazon, blogs, social media) before final report generation.
* **Tools:**
  - **Mistral AI Agents:** Used for data processing, product classification, and attribute extraction (cleaning raw data into structured insights).
  - **Extern API:** Collects social media (Pinterest, Instagram) and blog trend signals.
  - **HTTP Request / HTML Extract:** Used for web scraping to pull product listings and details from Amazon.
  - **Hugging Face (FLUX):** Generates photorealistic moodboard-style images for the identified trend segments.
  - **Google Drive:** Used in the final stages to store and organize the generated trend reports.


---

## 📄 License
This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.
