# 🧠 AI Agents — Learning How to Build AI Agents

This project is a hands-on exploration of how to build and orchestrate intelligent AI agents using modern tools like Hugging Face, Python, and LLMs. Inspired by OpenAI’s [Practical Guide to Building Agents](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf), this repo documents my learning journey from simple agent loops to more complex multi-agent systems.

---

## 🤖 What Are AI Agents?

AI agents are LLM-powered systems that **reason through tasks**, **make decisions**, and **take action** on the user's behalf. Unlike traditional automation, agents:

- Leverage language models to manage workflows
- Choose from a set of tools (APIs, functions) to act
- Follow clear instructions and guardrails
- Can orchestrate multi-step or multi-agent processes

This makes them ideal for tasks involving complex decisions, unstructured data, or workflows that are too brittle for simple rules.

---

## 🎯 Project Goals

- Understand the core components of agent design:
  - **Model**: The LLM powering reasoning
  - **Tools**: Functions that let the agent interact with the outside world
  - **Instructions**: Prompts, guidelines, and behavioral rules
- Practice building:
  - ✅ Single-agent loops
  - ✅ Tool selection via LLM
  - ✅ Multi-agent handoffs
  - 🚧 Guardrails and failure handling (coming soon)
- Compare architectures (single-agent vs multi-agent)
- Learn by building small, focused examples

---

## 📁 Current Examples

| Agent                     | Description                                              | Status  |
|--------------------------|----------------------------------------------------------|---------|
| `task_manager_agent`     | A single-agent system that saves, retrieves, and marks tasks as done | ✅ Complete |
| `customer_triage_agent`  | A triage agent that routes customer service messages to refund, sales, or tech agents | ✅ Complete |
| `multi_agent_handoff`    | Simulates multiple specialized agents working together    | ✅ Working |
| `guardrails_demo`        | Future example focused on handling edge cases & failures | 🚧 Coming Soon |

---

## 🛠️ Tools & Tech

- `transformers` by Hugging Face
- `flan-t5-base` (for lightweight text2text generation)
- Python + notebooks
- Git for version control
- OpenAI's design patterns and best practices

---

## 🧠 Based On: OpenAI’s Agent Design Guide

This repo is guided by [OpenAI’s Practical Guide to Building Agents (2024)](https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf), which outlines:

- When and why to use agents
- Core design principles (Model, Tools, Instructions)
- Orchestration strategies (single vs multi-agent)
- Guardrails and human-in-the-loop safety

All examples here follow those foundational patterns, adapted to open-source tools like Hugging Face and Python.

---

> ### Challenges of Building AI Agents
> While AI agents appear simple on the surface, building robust and reliable ones is hard. LLMs are inherently fuzzy — they don’t return strict formats, may hallucinate tools, and require careful prompt design. Even when structured examples are given, responses may deviate or be incomplete. Agents must be built to expect failure, validate every output, and fall back gracefully when things go wrong. This project highlights these challenges, and the work required to move from a simple chatbot to a real, resilient AI system.


