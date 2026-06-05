# LangGraph Agentic AI Playground

<p align="center">
  <strong>Hands-on LangGraph workflows, conversational AI experiments, and an MCP server starter.</strong>
</p>

<p align="center">
  Built with <strong>LangGraph</strong>, <strong>LangChain</strong>, <strong>Groq</strong>, and <strong>Tavily</strong>.
</p>

## Overview

This repository is a practical workspace for building and testing agentic AI systems with LangGraph. It includes notebook-driven experiments for chatbots and human-in-the-loop flows, plus a lightweight MCP server scaffold for tool-based integrations.

If you are a recruiter or technical reviewer, the main signal here is simple: this repo shows I can design, iterate on, and operationalize LLM-powered workflows end to end.

## What Is Inside

- `1-basic_chatbot/1-chatbot.ipynb` - a foundational LangChain + LangGraph chatbot notebook.
- `HumanAssistance/humanintheloop.ipynb` - a human-in-the-loop workflow exploration.
- `mcp_server/` - a separate Python package workspace for MCP server development.
- `main.py` - a minimal entry point for the root project.
- `pyproject.toml` and `uv.lock` - modern Python packaging and dependency management.

## Why This Repo Stands Out

- Agentic thinking: experiments are organized around graph-based control flow instead of one-off prompts.
- Tool use: the stack includes web search and model integration patterns for practical assistants.
- Human oversight: the repo explores human-in-the-loop design, which is critical for production AI systems.
- Reproducibility: dependencies are pinned and the workspace is configured for `uv`.

## Tech Stack

- Python 3.13+
- LangGraph
- LangChain
- Groq
- Tavily
- python-dotenv
- MCP server workspace support

## Getting Started

### 1. Create and activate the environment

```powershell
uv venv
.venv\Scripts\Activate.ps1
```

### 2. Install dependencies

```powershell
uv sync
```

### 3. Configure environment variables

Create a local `.env` file at the repo root with the API keys you need.

```env
GROQ_API_KEY=your_groq_key
TAVILY_API_KEY=your_tavily_key
```

### 4. Run the root project

```powershell
python main.py
```

### 5. Open the notebooks

Launch Jupyter or VS Code notebooks and explore the examples in `1-basic_chatbot/` and `HumanAssistance/`.

## Repo Structure

```text
langgraph/
├─ 1-basic_chatbot/
├─ HumanAssistance/
├─ mcp_server/
├─ main.py
├─ pyproject.toml
├─ requirements.txt
└─ uv.lock
```

## Notes For Reviewers

- Secrets are intentionally excluded from version control via `.gitignore`.
- This repo is a learning and experimentation workspace, so notebooks are the primary source of implementation detail.
- The project is structured to make it easy to extend into more advanced agents, tools, and server-side integrations.

## Next Steps

- Expand the chatbot notebook into a multi-tool assistant.
- Add a concise architecture diagram for the agent flow.
- Document the MCP server interface once its endpoints are finalized.
