AI Assistant
handles your emails , schedule , to-do lists , keeps you updated on Slack messages , and performs online research for you 🔍—all through your favorite messaging app.**

This project provides a personal assistant agent that manages tasks related to your email inbox, calendar, Notion to-do list, Slack interactions, and handles any research you may have. The assistant communicates with you via your preferred communication channel (Telegram, Slack, or WhatsApp), keeping you informed about your schedule, tasks, emails, messages, and helping with research topics, people, or even companies.

The personal assistant is a hierarchical multi-agents system with a supervisor agent (manager) and several sub-agents that handle specific tasks and tools for efficient task management.

Overview
Main Agent: Assistant Manager
The Assistant Manager is your personal assistant that orchestrates the tasks and communication between you and the sub-agents. The manager is responsible for:

Receiving and analyzing your messages from your chosen communication channel.
Delegating tasks to the appropriate sub-agent (Email, Calendar, Notion, Slack, or Researcher).
Communicating updates, messages, and any queries back to you via your preferred channel.
Tech Stack
LangGraph & LangChain: Frameworks used for building the AI agents and interacting with LLMs (GPT-4, Llama 3, Gemini).
LangSmith: For monitoring the different LLM calls and AI agents' interactions.
Google APIs: Provides access to Google services like Calendar, Contacts, and Gmail.
Notion Client: Interface for interacting with Notion to manage and update to-do lists.
Slack SDK: For interacting with Slack, sending and receiving messages.
Tavily Search API: For performing web searches.
Telegram API: Depending on your choice of communication channel.
WhatsApp API via Twilio Sandbox (for testing): A way to integrate WhatsApp communication.
How to Run
Prerequisites
Python 3.9+
Your preferred LLM provider API keys (OpenAI, Claude, Gemini, Groq,...)
Google API credentials (for Calendar, Contacts, and Gmail access)
Notion API key
Tavily API key (for web research)
Slack Bot User OAuth Token and App Token
Telegram Bot Token (If you want to use telegram)
Twilio Account SID and Auth Token (If you want to test with WhatsApp)
Necessary Python libraries (listed in requirements.txt)
