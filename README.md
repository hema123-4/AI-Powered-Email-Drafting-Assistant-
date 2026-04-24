# AI-Powered Email Drafting Assistant 📧🤖

An agentic AI workflow built with **LangGraph**, **LangChain**, and **Google Gemini** that automatically classifies incoming emails and generates context-aware draft replies.

## 🌟 Key Features
- **Agentic Workflow:** Utilizes a state-based graph architecture to manage email processing stages.
- **Intent Classification:** Automatically distinguishes between "Professional" and "Personal" communications.
- **Dynamic Drafting:** Generates tone-appropriate replies (formal vs. casual) based on the classification result.
- **Gmail Integration:** Uses the Google Gmail API to fetch unread messages and mark them as processed.
- **State Management:** Built with `TypedDict` to maintain context throughout the agent's lifecycle.

## 🛠️ Tech Stack
- **Orchestration:** [LangGraph](https://github.com/langchain-ai/langgraph)
- **LLM:** Google Gemini 1.5 Flash
- **Framework:** LangChain
- **API Integration:** Google Gmail API (OAuth2)
- **Language:** Python

## 📐 System Architecture
The project follows a directed acyclic graph (DAG) structure:
1. **Classify Node:** Labels the email intent.
2. **Draft Node:** Generates a tailored reply based on the label.
3. **Notify Node:** Formats a summary notification of the draft.

## 🚀 Getting Started

### Prerequisites
- Python 3.10+
- A Google Cloud Project with the Gmail API enabled.
- A `credentials.json` file from your Google Cloud Console.

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/hema123-4/AI-Powered-Email-Drafting-Assistant
