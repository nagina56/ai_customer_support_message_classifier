# AI Customer Support Message Classifier — n8n + Ollama

An AI-powered customer support message classification workflow built using **n8n, Ollama, and Gemma 3 4B**. This project analyzes customer messages and classifies them into relevant categories to help organize customer support requests.

## Project Overview

The AI Customer Support Message Classifier automates the process of understanding and categorizing incoming customer messages. Using a locally running language model, the workflow analyzes the message and identifies its most suitable support category.

This project demonstrates how AI and workflow automation can be combined to simplify customer support tasks.

## Features

- **Automated Message Classification:** Analyzes customer messages and assigns appropriate categories.
- **AI-Powered Analysis:** Uses an Ollama language model to understand message context.
- **Customer Support Categories:** Supports categories such as Technical Issue, Billing, Account Support, and General Inquiry, depending on the configured prompt.
- **Workflow Automation:** Connects workflow steps using n8n.
- **Local AI Processing:** Uses Gemma 3 4B through Ollama without requiring a paid OpenAI API.
- **Structured Output:** Presents classification results for review.
- **Potential for Integration:** Can be extended to store results in Google Sheets or connect to other support workflows.

## Technologies Used

- n8n
- Ollama
- Gemma 3 4B
- Basic LLM Chain
- Prompt Engineering
- AI Workflow Automation

## How It Works

1. **Message Input:** The workflow receives a customer support message through its configured input method.
2. **AI Processing:** The message is passed to a Basic LLM Chain.
3. **Message Classification:** The Ollama model analyzes the message and determines the appropriate category.
4. **Result Output:** The classification result is returned by the workflow for review.

## Example

**Customer Message:**

"I cannot log in to my account even after resetting my password."

**Possible Classification:**

- Category: Account Support
- Reason: The customer is experiencing a login problem after resetting their password.

*The actual output depends on the workflow prompt and the AI model's response.*

## Setup and Usage

### Prerequisites

- n8n
- Ollama
- Gemma 3 4B model

### Steps

1. Install and run Ollama.
2. Download the model:

   ```bash
   ollama pull gemma3:4b
   ```

3. Start your local n8n instance.
4. Import the workflow JSON file into n8n, if included in this repository.
5. Configure the Ollama Chat Model node and its credentials.
6. Review the Basic LLM Chain prompt and connect the required nodes.
7. Execute the workflow and submit a sample customer message.
8. Review the classification result.

## Use Cases

- Organizing customer support messages
- Identifying technical issues
- Categorizing billing questions
- Classifying account-related problems
- Supporting customer service automation

## Learning Outcomes

By building this project, I practiced:

- Creating AI workflows in n8n
- Connecting a local LLM through Ollama
- Writing structured prompts for classification
- Processing customer messages using AI
- Testing and debugging automation workflows

## Future Improvements

- Save classification results to Google Sheets.
- Add priority detection for urgent customer messages.
- Support multilingual customer messages.
- Integrate with email or customer support platforms.
- Route messages to the appropriate support team.

## Author

**Nagina Azhar**

Building practical projects in AI, Python, and workflow automation.

---

*Created for learning, experimentation, and portfolio development.*
