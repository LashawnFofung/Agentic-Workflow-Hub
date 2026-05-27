# Lab 04 Designing the AI Insights & Content Agent

[View JSON](https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/N8N%20Workflow/Content%20Strategy%20AI%20Agent.json)

[View Content Strategy Report]()

-----


## 📌 Overview & Business Purpose
* **Core Objective:** Reverse-engineered and enhanced an inherited n8n-based AI Content Engine to synthesize market trends (Project 2) and competitor analysis (Project 3) into highly actionable, brand-aligned marketing assets.
* **Tech Stack:** n8n (Workflow Automation), Mistral AI (`mistral-large-latest`), JavaScript/HTML5/CSS3.

---

## 📐 Base Workflow Architecture
The system orchestrates data through **7 core stages**:
1. **Upload Form:** Captures product categories and imports HTML reports.
2. **Extract Files:** Strips HTML formatting into structured plain text.
3. **AI Content Node (Mistral):** Uses role-based system prompts to enforce strict JSON schemas.
4. **Parse Content:** Standardizes the JSON output to eliminate downstream parser errors.
5. **Build HTML:** Dynamically renders the parsed JSON into a themed document.
6. **Download / Preview:** Outputs the file via local download or inline browser preview.

---

## 💡 Implemented Enhancements (Collaborative Design Engine)
* **User Input Personalization:** Expanded the input form with dropdown selectors for **Style Persona** (e.g., Minimalist, Maximalist) and text fields for custom **Vibe Keywords**.
* **Prompt Engineering Guardrails:** * Implemented a strict **Anti-AI-ism Filter** to remove generic corporate fluff and AI jargon.
  * Extended the system prompt to return a mandatory `mood_board_assets` JSON object filled with color hex codes, tactile descriptions, and furniture layout ideas.
* **UI/UX App Conversion:** Upgraded the static `Build HTML` template into an interactive, 3-tab user dashboard client (`Strategy`, `Design`, `Creative`).
  * Added active state tracking widgets (`To Do`, `Drafting`, `Ready`) via browser LocalStorage.
  * Embedded a dynamic JavaScript click-to-copy utility for quick caption/headline exporting.

---

## 🧠 Key Takeaways & Reflection
* **AI Engineering Level-Up:** Mastered advanced prompt engineering structures specifically optimized for strict JSON generation over multi-variable datasets.
* **System Constraints:** Learned to effectively pair strict validation layers (JSON formatting parameters) with creative text boundaries (Anti-AI-ism filters) to ensure both functional stability and human-like output tone.
