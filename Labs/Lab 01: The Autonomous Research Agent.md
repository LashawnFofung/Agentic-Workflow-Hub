# 🧪 Lab 01: Getting Started with AI Agents – Moodboard Generator

## AI Agent Workflows
- ["Hello World!"](https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Labs/Lab%2001:%20The%20Autonomous%20Research%20Agent.md#hello-world)

- []()

----

### Hello World!

This "Hello World" lab is a foundational exercise designed to verify that your n8n environment is correctly installed and configured. By building this simple workflow, you confirm that you can create nodes, configure them, and successfully execute an end-to-end process.

**Lab Summary: Hello World in n8n**

- <b>Objective:</b> The primary goal is to validate your development environment by displaying a "Hello World!" message. This provides immediate confirmation that the system is operational.

- <b>Key Tasks:</b>

  - Initialize a new workflow within the n8n interface.
  
  - Add a Manual Trigger node to initiate the workflow manually.
  
  - Configure a Code node to return the string: {"message": "Hello World!"}.
  
  - Execute the workflow and inspect the output in the n8n interface to verify successful delivery.

- <b>Why It Matters:</b> While simple, this exercise is a standard "passing ritual" for developers. It ensures your toolchain (editor, interpreter, and execution environment) is working correctly before you attempt to build more complex, agentic automations.

This lab serves as your first step toward becoming a "flow programmer," helping you get comfortable with the n8n canvas and data flow before you move on to advanced agentic workflows.

![Hello World!](https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Lab%20Artifacts/Lab%201/Hello%20World%20Message%20Workflow%20screenshot.png)

<b>View DEMO:</b> [HERE](https://youtu.be/hCA3ZIhQVc8)

<h1></h1>

### My First AI Agent with N8N: Conditional Flow

In this lab, I walk through the fundamentals of n8n workflow automation by focusing on four key areas:

- <b>Trigger Management:</b> Setting up schedules to act as an agent's "heartbeat."

- <b>Data Transformation:</b> Using the Code Node to inject and manipulate JSON data.

- <b>Conditional Logic:</b> Implementing If nodes to evaluate information.

- <b>Branching Workflows:</b> Executing different actions based on real-time data analysis.

The lab is structured as a logical flow, beginning with a Schedule Trigger to define my automation frequency, followed by a Code Node that simulates a data source, such as weather conditions. From there, I utilize an If Node as a logic engine to evaluate that data—for instance, checking if the weather is "sunny"—and finally, I connect Set Nodes to define distinct branching outcomes, such as sending a bright message for sunny days or a calmer one for cloudy conditions.

<br>

<b>💡 The Learning Outcome:</b> By following these steps, I can visualize how data flows through the system and how my logic dictates the final output. This process ensures that I am not just building a static script, but a dynamic, decision-making workflow that serves as the foundation for the more advanced autonomous agents I plan to build later.


![My First AI Agent with N8N](https://github.com/LashawnFofung/Agentic-Workflow-Hub/blob/main/Lab%20Artifacts/Lab%201/My%20First%20AI%20Agent.png)

<b>View DEMO:</b> [HERE](https://youtu.be/FcLEMod7w-M)




