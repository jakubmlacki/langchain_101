# LangChain & LangGraph Basics (Polish → English)

This repository contains a set of Jupyter notebooks introducing core concepts of **LangChain** and **LangGraph**.  
All user-facing text (comments, prompts, prints, and markdown) has been converted to **English** so the materials are understandable to a wider audience.

## Notebooks Overview

1. **01_basic_llm.ipynb** — Call an LLM, construct simple prompts, and run basic invocations.
2. **02_structured_output.ipynb** — Generate structured outputs (e.g., JSON-like responses) and parse model outputs safely.
3. **03_langgraph.ipynb** — Build a minimal LangGraph, define nodes/edges, and execute the graph.
4. **04_langgraph_with_fork.ipynb** — Add branching to your graph (forks), route between nodes, and handle multiple paths.
5. **05_langgraph_with_fork_memory.ipynb** — Extend the forked graph with memory/state to preserve context across steps.

> Note: The exact code focuses on clarity. Prompts are intentionally concise and generic so you can adapt them to your use case.

## Getting Started

### Prerequisites
- Python 3.10+
- Jupyter Notebook or JupyterLab
- A supported LLM provider/API key (e.g., OpenAI). Set environment variables as needed (e.g., `OPENAI_API_KEY`).

### Installation
```bash
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
pip install -U pip
pip install -r requirements.txt  # or: pip install langchain langgraph jupyter
```

> If you do not keep a `requirements.txt`, install the dependencies you see imported at the tops of the notebooks.

### Running
```bash
jupyter lab  # or: jupyter notebook
```

Open each notebook in order and run the cells from top to bottom. Where credentials are needed, ensure your environment variables are set before running.

## Notes on Prompts & Safety
- All prompts are generic, minimal, and **English-only**. Tailor them to your data and domain for best results.
- For structured outputs, validate and handle parsing errors defensively.
- Use smaller test inputs first; scale up once the pipeline/graph behaves as expected.

## License
MIT (or your preferred license).