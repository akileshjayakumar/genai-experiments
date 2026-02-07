# GenAI Experiments

Notebook-first experiments for learning agent workflows with Google ADK, OpenAI Agents SDK, and Prefect.

## Quick Start

### Prerequisites
- Python 3.10+
- JupyterLab or Jupyter Notebook

### Setup
```bash
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip notebook jupyterlab python-dotenv
```

### Run
```bash
jupyter lab
```

Open one of the notebooks:
- `google-adk/notebooks/agent.ipynb`
- `openai-agents-sdk/notebooks/agent.ipynb`
- `prefect/notebooks/main.ipynb`

## Features
- Google ADK example agent with Google Search tooling
- OpenAI Agents SDK notebook with guardrail and runner examples
- Prefect notebook showing simple flows/tasks and dataset processing

## Configuration
- `OPENAI_API_KEY`: required for `openai-agents-sdk/notebooks/agent.ipynb`
- `GOOGLE_API_KEY` or `GEMINI_API_KEY`: required for `google-adk/notebooks/agent.ipynb`

Example:
```bash
export OPENAI_API_KEY="your_key_here"
export GOOGLE_API_KEY="your_key_here"
```

## Usage
Install per-notebook dependencies in notebook cells:
- Google ADK notebook: `%pip install google-adk`
- OpenAI Agents notebook: `%pip install openai-agents`
- Prefect notebook: `%pip install prefect datasets matplotlib`

## Contributing and Validation
```bash
python -m py_compile google-adk/my_agent/agent.py
```

For notebook changes, rerun cells top-to-bottom and ensure no exceptions.

## License
MIT. See `LICENSE`.
