Gmail Draft Creator Workflow
This repository contains a workflow designed to automate the process of classifying incoming emails and drafting automated, professional responses based on their content. The workflow uses a Large Language Model (LLM) to intelligently analyze emails and generate context-aware replies.

🚀 How It Works
This workflow operates on a simple, linear process:

Email Ingestion: The workflow is triggered by a new email received in a connected Gmail account.

AI Classification: An LLM classifies the email into a predefined category, such as Sponsorship or High Priority. This step helps route the email to the correct handling process.

AI Response Generation: Based on the classification, the LLM drafts a full email response, including a subject line and a body. The AI is instructed to format this response as a JSON object to ensure clean, structured output.

Data Parsing: A small code node parses the AI's JSON-formatted text output into a usable data object, separating the subject and body.

Draft Creation: The final step uses the parsed data to automatically create a new draft email in the user's Gmail account, ready for review and sending.

✨ Features
Intelligent Classification: Uses a powerful LLM to accurately categorize emails.

Automated Drafting: Generates full email responses with both a subject and a body.

Structured Output: Ensures clean data handling by instructing the AI to output JSON.

Customizable: Easily adaptable to new email categories, different tones, and varied response formats by simply changing the AI's instructions.

🔧 Getting Started
To use this workflow, you will need to import it into your preferred workflow automation platform (e.g., n8n, Zapier, Make).

Set up the Gmail Trigger: Connect your Gmail account and configure the trigger to watch for new emails.

Configure the LLM: Connect the LLM (e.g., Google Gemini) and provide the system prompts for the AI to follow.

Add the JSON Parsing Node: Include a code node with the provided JavaScript to parse the AI's output.

Connect to the Gmail Node: Use the parsed subject and body from the code node to create the final email draft.

💡 Contributions
This is a simple template to get started. Feel free to fork this project and customize it for your specific needs!

📜 License
This project is open-source.
