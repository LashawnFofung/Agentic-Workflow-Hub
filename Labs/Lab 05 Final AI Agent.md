# Lab 05 Bringing It All Together: Final AI Agent in Action

## 📌 Project Overview & Objectives

**Core Objective:** Unify independent analytical outputs from previous stages into a single, centralized, decision-ready Market Intelligence Dashboard

**Business Purpose:**
- Eradicate data isolation
- Instead of forcing Wayfair category managers and leadership to cross-reference disconnected reports, this agent automates live data retrieval to generate a single executive briefing document in under a minute.

---

## 🛠 Tech Stack & Integration Components
- **Workflow Automation Engine:** n8n 
- **Upstream Agents Integrated:** Project 2 (Market Trend Discovery Agent) & Project 3 (Competitor Monitoring Agent) 
- **HTML Dom Parser Library:** Cheerio (for custom structured web scraping text extraction) 
- **Cloud Storage Protocol:** Google Drive API via OAuth2 authentication 
- **Client UI Environment:** Responsive HTML5, CSS Grid/Flexbox layouts, Vanilla JavaScript 

---

## 📐 Consolidated Data Flow & Architecture
The system ceases working in isolation and transforms into an end-to-end extraction and rendering pipeline across several key stages:

### Phase A: Upstream Hardening (Modifications to P2 & P3)
1. **Stealth Header Injections:** Upgraded upstream HTTP Request nodes in Project 2 and Project 3 with comprehensive browser headers (`User-Agent`, `Accept-Language`, `Device-Memory`) to bypass anti-bot defenses on Amazon and Walmart.
2. **Automated Folder Provisioning:** Configured n8n sub-flows to dynamically search, verify, and create an organized folder structure inside Google Drive: `Wayfair Reports` ➔ `[Category]` ➔ `[YYYY-MM-DD]`.
3. **Automated Payload Sync:** Programmed the final nodes of P2 and P3 to upload their raw binary HTML report outputs straight to their respective date folders.

### Phase B: The Dashboard Builder Agent Pipeline

[Google Drive Setup] ➔ [Fetch Latest Date Folder] ➔ [Download P2/P3 Binaries] ➔ [Cheerio Extraction Node] ➔ [Template Compilation] ➔ [HTML/PDF Output]

1. **Latest Log Resolution:** The workflow scans the targeted category folder alphabetically, filtering out obsolete folders to return only the single most recent date log folder ID.
2. **Asynchronous Binary Fetching:** Simultaneously pulls down three files from Drive: the clean baseline dashboard boilerplate template, the latest P2 HTML trend report, and the latest P3 HTML competitor report.
3. **Cheerio Extraction Engine:** Executes a JavaScript `Code` node utilizing Cheerio selectors to parse unstructured HTML text arrays into cleanly formatted JSON data objects:
   - *P2 Extraction:* Captures micro-segments, target color swatches, market sizes, CAGRs, and risks.
   - *P3 Extraction:* Captures product count metrics, competitor pricing discrepancies, stock gaps, and supplier metadata.
4. **Dynamic Value Injection:** Uses a dynamic regex helper loop function (`/g` flag substitution) to swap design placeholders inside the dashboard template with the freshly parsed structured data string values.

---

## 💡 Implemented Enhancements & Custom Modifications
*Modify this section to match any personal design tweaks you applied during the prompt or layout modules:*

- **Strategic Multi-Tab Layout:** Structured the final output dashboard with a responsive navigation sidebar breaking data down into `📊 Overview`, `📈 Market Trends`, and `🔍 Competitor Insights` layouts.
- **Visual Color Swatch Cards:** Mapped text string color names extracted by Cheerio directly into raw CSS background-color styles, enabling physical color swatch renders on the category summary panel.
- **Parser Failure Fallbacks:** Implemented standard fallback strings (e.g., `<p class="empty-state">No recommendations available</p>`) to safeguard layout architecture if an upstream file has missing data fields.

---

## 🧠 Key Takeaways & Reflection
- **Architect of Intelligence:** Shifted from simply utilizing pre-packaged tools to architecting connected intelligence ecosystems. The major value add isn't in generating a single report, but in establishing automated data pipelines that can constantly repeat without manual engineering intervention.
- **Data Synthesis Mastery:** Learned how to treat output HTML reports from one AI engine as structured input databases for another by leveraging automated DOM query selectors (Cheerio) and n8n binary manipulation tools.
