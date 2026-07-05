# AI Business Analytics Assistant

![Python](https://img.shields.io/badge/Python-3.9+-3776AB?logo=python&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1.0.3-blue)
![Chainlit](https://img.shields.io/badge/Chainlit-2.9.0-orange)
![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o--mini-green)
![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?logo=sqlite)
![Plotly](https://img.shields.io/badge/Plotly-Interactive_Charts-purple)
![License](https://img.shields.io/badge/License-MIT-success)

An intelligent multi-agent AI system that transforms natural language questions into SQL queries, executes them on an e-commerce database, analyzes the results, and automatically generates interactive visualizations using LangGraph, Chainlit, OpenAI, SQLite, and Plotly.

---

# Overview

Business users often need insights from databases without knowing SQL.

This project demonstrates how multiple specialized AI agents can collaborate to translate natural language into SQL, execute database queries, recover from SQL errors, analyze the results, and generate interactive business visualizations.

Rather than acting as a traditional chatbot, the system orchestrates a team of specialized agents to perform a complete business analytics workflow.

---

# System Architecture

![Workflow](text2sql_workflow.png)

The assistant follows a LangGraph-based workflow consisting of specialized AI agents.

Workflow:

1. Validate user request
2. Generate SQL query
3. Execute SQL
4. Recover from SQL errors (if needed)
5. Analyze query results
6. Decide whether visualization is required
7. Generate interactive Plotly charts
8. Return business insights

---

# Key Features

✅ Natural Language → SQL conversion

✅ Multi-Agent architecture using LangGraph

✅ SQL error detection and automatic recovery

✅ Business insight generation

✅ Interactive Plotly visualizations

✅ Guardrails for out-of-scope questions

✅ Streaming agent execution with Chainlit

✅ SQLite backend

---

# Agent Workflow

The application consists of several specialized AI agents.

## Guardrails Agent

- Validates whether questions are related to the business database.
- Rejects out-of-scope requests.
- Handles greetings and general conversation.

---

## SQL Agent

- Converts natural language into optimized SQLite queries.
- Understands database schema.
- Generates syntactically correct SQL.

---

## SQL Execution Agent

- Executes SQL against the SQLite database.
- Returns structured query results.
- Handles multiple SQL statements.

---

## Error Recovery Agent

- Detects SQL execution failures.
- Repairs incorrect SQL.
- Retries execution automatically.

---

## Analysis Agent

- Converts structured query results into business insights.
- Generates concise natural language explanations.

---

## Visualization Agent

- Determines whether charts improve understanding.
- Creates interactive Plotly visualizations.
- Supports multiple chart types.

---

# Example Questions

Users can ask questions such as:

- How many orders were delivered?
- Which sellers generated the highest revenue?
- Show top selling product categories.
- What is the average review score?
- Compare monthly sales.
- Which states have the highest number of customers?
- Show payment type distribution.
- Which products generate the highest revenue?

---

# Technology Stack

## AI

- OpenAI GPT-4o-mini
- LangGraph
- Prompt Engineering
- Multi-Agent Systems

## Backend

- Python
- SQLite
- Pandas

## Frontend

- Chainlit

## Visualization

- Plotly

---

# Repository Structure

```text
AI-Business-Analytics-Assistant/

├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
│
├── app.py
├── text2sql_agent.py
├── db_init.py
│
├── agentic_text2sql_analytics.ipynb
│
└── text2sql_workflow.png
```

---

# Installation

Clone the repository.

```bash
git clone https://github.com/AShirsat96/AI-Business-Analytics-Assistant.git
```

Install dependencies.

```bash
pip install -r requirements.txt
```

Download the **Olist E-commerce Dataset** from Kaggle and place the CSV files inside a folder named:

```text
data/
```

Create the SQLite database.

```bash
python db_init.py
```

Start the application.

```bash
chainlit run app.py
```

---

# Skills Demonstrated

This project demonstrates practical experience with:

- Multi-Agent AI Systems
- LangGraph Workflow Orchestration
- Text-to-SQL Systems
- Prompt Engineering
- SQL Generation
- Error Recovery Workflows
- Business Analytics
- Data Visualization
- SQLite
- Plotly
- Chainlit
- OpenAI API

---

# Future Improvements

Potential future enhancements include:

- Support for PostgreSQL and MySQL
- Database schema auto-discovery
- Role-based access control
- Vector memory for conversation history
- Multi-database support
- Dashboard export
- Docker deployment
- Cloud deployment
- Authentication
- Query optimization

---

# Project Context

This project demonstrates an enterprise-style AI business analytics workflow using a multi-agent architecture.

The system showcases how specialized AI agents can collaborate to automate SQL generation, business analysis, error recovery, and visualization within a single conversational interface.

---

# About the Author

**Aniket Shirsat**

AI Engineer | Data Scientist | Generative AI

🌐 Portfolio  
https://aniketdshirsat.com

💼 LinkedIn  
https://www.linkedin.com/in/aniketshirsatsg/

📧 Email  
aniketdshirsat@hotmail.com

---

# License

This project is licensed under the MIT License.
