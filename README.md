# 📰 Bayelsa News AI Automation.

An AI-powered news automation platform built with **n8n, WhatsApp Business Cloud API, Supabase, Gemini, and The News API**.

The system collects Bayelsa State news, cleans and processes the articles, stores them in a database, delivers news to WhatsApp subscribers, and allows users to ask questions about available Bayelsa news.

## 🚀 Project Overview

Bayelsa News AI was built to automate the complete news workflow:

**Collect → Clean → Validate → Store → Process → Deliver → Interact**

The platform is designed with reliability, data validation, error handling, and human oversight in mind.

## 🏗️ Architecture

```text
                    NEWS SOURCES
                         │
                         ▼
                ┌─────────────────┐
                │  News Collector │
                │     (n8n)       │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │ Data Cleaning & │
                │   Validation    │
                └────────┬────────┘
                         │
                         ▼
                ┌─────────────────┐
                │    Supabase     │
                │   News Database │
                └────────┬────────┘
                         │
             ┌───────────┴───────────┐
             ▼                       ▼
     Daily News Delivery       AI Conversation
             │                       │
             ▼                       ▼
        WhatsApp                Gemini AI
             │                       │
             └───────────┬───────────┘
                         ▼
                    WhatsApp Users
```

## ⚙️ Main Features

* 📰 Automated Bayelsa news collection
* 🧹 JavaScript-based data cleaning
* 🔎 Duplicate article detection
* 🗄️ Supabase database storage
* 📱 WhatsApp Business integration
* 🤖 AI-powered news conversations
* 💬 Subscriber commands
* 📅 Daily news delivery
* 🔗 Article source links
* 🛡️ Input validation and safety rules
* 🚨 Error handling and recovery workflow
* 📊 Subscriber management
* 🔄 Separate workflows for collection, processing, delivery, and conversation

## 📱 WhatsApp Commands

Subscribers can interact with the system using commands such as:

```text
START
STOP
NEWS
HELP
```

Users can also ask natural-language questions such as:

```text
What is the latest Bayelsa news?
What happened in Bayelsa today?
Tell me about recent developments in Bayelsa.
```

## 🧠 AI Conversation

The AI conversation workflow uses Gemini to answer questions using the available processed Bayelsa news.

The system is designed to avoid inventing information when the database does not contain enough information to answer a question.

Each response can reference the original news source and article URL when available.

## 🗃️ Database

The project uses **Supabase** for persistent data storage.

The database includes information such as:

* News articles
* Subscribers
* Article metadata
* Publication dates
* News categories
* Sources
* Processing status
* Subscriber status

## 🔄 n8n Workflows

The project is organized into multiple workflows:

| Workflow | Purpose                     |
| -------- | --------------------------- |
| V1       | Real-Time News Collector    |
| V2       | News Processor              |
| V3       | Database Core & Reliability |
| V4       | WhatsApp Receiver           |
| V5       | Daily News Delivery         |
| V6       | AI News Conversation        |
| V7–V10   | Facebook Publishing         |
| V11      | Error Handling & Recovery   |

## 🛠️ Technology Stack

* **n8n** — Workflow automation
* **JavaScript** — Data processing and validation
* **Python** — Planned data-processing/automation support
* **Gemini API** — AI conversation
* **WhatsApp Business Cloud API** — Messaging
* **Supabase** — Database
* **The News API** — News collection
* **GitHub** — Source control and documentation
* **Facebook** — Planned publishing channel

## 🔐 Security

Secrets and API credentials are **not stored in this repository**.

Examples of sensitive information that should remain private:

* API keys
* WhatsApp access tokens
* Supabase service keys
* Database passwords
* Webhook secrets
* Environment variables

## 📚 What This Project Demonstrates

This project demonstrates practical experience with:

* REST APIs
* Webhooks
* JSON
* HTTP requests
* API authentication
* JavaScript
* Database design
* Supabase
* n8n workflow automation
* AI integration
* WhatsApp Business API
* Data validation
* Error handling
* Automation reliability
* GitHub project management

## 🎯 Project Goal

The goal of Bayelsa News AI is to demonstrate how multiple technologies can be combined into a reliable AI automation system that collects information, processes data, stores structured records, and communicates with users through WhatsApp.

## ⚠️ Disclaimer

This project is an educational and portfolio automation project.

News information originates from external news sources. Users should consult the original source links for the full article and additional context.

## 👨‍💻 Author

**Prince Pere-Ebi Kumokou**

AI Automation Developer

---

⭐ If you find this project interesting, feel free to explore the workflow architecture and technologies used.
