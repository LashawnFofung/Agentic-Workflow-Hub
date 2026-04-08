# 🧪 Lab 03 Building the Competitor Monitoring AI Agent


  ## Objective:
This lab showcases the integration of multi-modal LLMs and low-code orchestration to transform raw market data into actionable retail insights.

<br>

  <b>View DEMO Stages & Node Execution Walkthough:</b> [HERE](https://youtu.be/gi0bSrUmX9E)

  <b> View JSON:</b> [HERE](https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/N8N%20Workflow/Competitor%20Monitoring%20AI%20Agent.json)

  <b> View Competitor Analysis Report</b> [HERE](https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Lab%20Artifacts/Lab%203/Competitor%20Analysis%20Report%20-%20Area%20Rugs.pdf)

<h1></h1>

## Workflow Architecture:
- **Stage 1:** Input Parsing: Processes target URLs and categories via JavaScript.
- **Stage 2:** Wayfair Scraping: Scrapes internal Wayfair data to set comparison metrics.
- **Stage 3:** Amazon Scraping (Dual Path): Parallel extraction of individual product specs and category-wide collection trends.
- **Stage 4:** Walmart Scraping : Targeted scraping of Walmart’s retail data to complete the competitive landscape.
- **Stage 5:** AI Analysis & Report Generation (Multi-Model Analysis): Uses Gemini 2.0 and Mistral Large to synthesize pricing heatmaps and "whitespace" gaps.
- **Stage 6:** Report Generation

<br>

## Technical Highlights:
- **Dynamic Scraping:** Uses HTTP Request and Cheerio nodes to handle diverse HTML structures.
- **Rate Management:** Integrated Wait Nodes to ensure stable execution across multiple API calls.
- **Agentic Reporting:** Automatically generates a styled HTML report stored in Google Drive.


## Workflow Images

**Stage 1: Input & Routing**

<img src=https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Lab%20Artifacts/Lab%203/Stage%201%20Input%20%26%20Routing.png width="700" height="600" alt="Stage 1">

<br>


**Stage 2: Wayfair Scraping**

<img src=https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Lab%20Artifacts/Lab%203/Stage%202%20Wayfair%20Scraping.png width="900" height="800" alt="Stage 1">
  
  <br>

**Stage 3: Amazon Scraping (Dual Path)**

<img src=https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Lab%20Artifacts/Lab%203/Stage%203%20Amazon%20Scraping.png width="900" height="800" alt="Stage 1">

<br>

**Stage 4: Walmart Scraping**

<img src=https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Lab%20Artifacts/Lab%203/Stage%204%20Walmart%20Scraping.png width="900" height="800" alt="Stage 1">

<br>

**Stage 5: AI Analysis & Report Generation Part 1**

<img src=https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Lab%20Artifacts/Lab%203/Stage%205%20AI%20Analysis%20%26%20Report%20Generation%20Part%201.png width="900" height="800" alt="Stage 1">

<br>

**Stage 5: AI Analysis & Report Generation Part 2**

<img src=https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Lab%20Artifacts/Lab%203/Stage%205%20AI%20Analysis%20%26%20Report%20Generation%20Part%202.png width="900" height="800" alt="Stage 1">

<br>

**Stage 6: Report Assembly**

<img src=https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Lab%20Artifacts/Lab%203/Stage%206%20Report%20Assembly.png width="900" height="800" alt="Stage 1">

<br>
