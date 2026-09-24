# Langflow Web Research Agent

An AI-powered web research agent built using **Langflow** and **Google Gemini**. The agent can understand user queries, search the web for relevant information, retrieve webpage content, and generate contextual responses.

---

## 📌 Project Overview

This project demonstrates an **Agentic AI workflow** created using Langflow.

The system uses Google Gemini as the language model and provides the AI Agent with external tools for web research.

The agent can decide when it needs to use web-based tools to answer a user's query.

---

## 🏗️ Architecture

```text
                    ┌─────────────────┐
                    │   Chat Input    │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │    AI Agent     │
                    └────────┬────────┘
                             │
                ┌────────────┴────────────┐
                │                         │
                ▼                         ▼
       ┌─────────────────┐       ┌─────────────────┐
       │   Web Search    │       │      URL        │
       │      Tool       │       │  Content Tool   │
       └─────────────────┘       └─────────────────┘
                │                         │
                └────────────┬────────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │ Google Gemini   │
                    │ Language Model  │
                    └────────┬────────┘
                             │
                             ▼
                    ┌─────────────────┐
                    │   Chat Output   │
                    └─────────────────┘