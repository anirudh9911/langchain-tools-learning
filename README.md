# LangChain Tools Learning

A hands-on notebook exploring how **Tools** work in [LangChain](https://python.langchain.com/) — from built-in tools to fully custom ones, plus grouping them into toolkits.

## Contents (`tools_in_langchain.ipynb`)

- **Built-in Tool — Web Search**: using `DuckDuckGoSearchRun` to run live web searches.
- **Built-in Tool — Shell Tool**: running shell commands via `ShellTool`.
- **Custom Tools**: building a tool step by step with the `@tool` decorator (plain function → type hints → decorator).
- **Method 2 — Structured Tools**: defining tool input schemas with Pydantic `BaseModel` and `StructuredTool.from_function`.
- **Method 3 — BaseTool**: subclassing `BaseTool` for full control over a tool's behavior.
- **Toolkits**: grouping related tools (e.g. `add`, `multiply`) into a reusable toolkit class.

## Setup

```bash
python -m venv .venv
source .venv/bin/activate  # on Windows: .venv\Scripts\activate
pip install -r requirements.txt
```

Create a `.env` file in the project root with any API keys required by the integrations you use (OpenAI, Anthropic, Google Gemini, Hugging Face, etc.):

```
OPENAI_API_KEY=your-key-here
ANTHROPIC_API_KEY=your-key-here
GOOGLE_API_KEY=your-key-here
```

## Usage

Open the notebook and run the cells in order:

```bash
jupyter notebook tools_in_langchain.ipynb
```

## Requirements

See [requirements.txt](requirements.txt) — includes LangChain core/community packages plus integrations for OpenAI, Anthropic, Google Gemini, and Hugging Face.
