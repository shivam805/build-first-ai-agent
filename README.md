# Build Your First AI Agent Using Python

Learn how to build your first AI Agent using Python, LangChain, and LangGraph concepts. This beginner-friendly project demonstrates how an AI Agent understands user instructions, decides which tools to call, performs actions, and returns results.

## 🚀 Project Overview

In this project, we build an AI Agent that can understand natural language instructions and check vehicles based on user-defined rules.

For example:
- Find bikes with a top speed greater than 300 km/h.
- Find cars with power greater than 1000 HP.
- Create custom vehicle rules and check which vehicles match.

## 🛠️ Technologies Used

- Python
- LangChain
- LangChain Agents
- LangGraph
- OpenAI GPT-4o-mini
- Pydantic

## 📦 Installation

Install the required Python libraries:

```python
%pip install -q -U langchain langchain-openai langgraph pydantic
```

## 🔑 OpenAI API Key Setup

You need an OpenAI API key to run this project.

```python
import os
from getpass import getpass

if not os.getenv("OPENAI_API_KEY"):
    os.environ["OPENAI_API_KEY"] = getpass("OpenAI API key: ")
```

## 🤖 Project Workflow

The AI Agent uses two tools:

### 1. Create Rule – AI Rule Generator

- Understands the user's natural language instruction.
- Converts the instruction into a structured rule.
- Saves the generated rule for further processing.

### 2. Check Vehicles – Python Rule Engine

- Reads the saved rule.
- Checks vehicle specifications.
- Identifies matching vehicles.
- Returns PASS or FAIL results.

## 🔄 AI Agent Execution Flow

```text
          User Input
               |
               v
           AI Agent
               |
        Understand Request
               |
          Tool Selection
               |
        +------+------+
        |             |
        v             v
    Create Rule   Check Vehicles
        |             |
        v             v
    AI Rule       Python Rule
    Generator       Engine
        |             |
        +------+------+
               |
               v
         Tool Results
               |
               v
        Final AI Response
```

## 💡 Example Inputs

Try these instructions:

**Example 1:**
```text
A fast bike has top speed over 300 km/h
```

**Example 2:**
```text
A powerful car has more than 1000 hp
```

**Example 3:**
```text
Check vehicles using the fast bike rule
```

## 🎯 What You Will Learn

- What is an AI Agent?
- How to create an AI Agent using Python.
- How to define and register tools.
- How an AI Agent selects tools.
- How to use structured output with Pydantic.
- How to combine AI decisions with Python logic.
- How to execute actions based on user instructions.
- How to build practical Agentic AI applications.

## 📚 Learning Resources

Explore the complete source code and run the notebook:

**GitHub Repository:**  
https://github.com/shivam805/build-first-ai-agent

## 👨‍💻 About This Project

This project is designed for beginners who want to learn Python, Generative AI, AI Agents, and Agentic AI through practical coding examples.

Learn step by step, build real-world projects, and prepare for AI Developer and GenAI Developer interviews.

**Keep Learning | Keep Building | Keep Growing!** 🚀

#Python #AIAgents #GenAI #AgenticAI #LangChain #LangGraph #OpenAI #PythonProjects #AIInterview
