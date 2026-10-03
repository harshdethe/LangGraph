# 🕸️ LangGraph Learning Projects

A hands-on collection of notebooks that walk through [LangGraph](https://langchain-ai.github.io/langgraph/) step by step, from a simple sequential graph to LLM workflows, conditional routing, parallel execution, loops, chatbots, persistence, and human-in-the-loop (HITL).

Each notebook is a small, self-contained example that builds on the previous one.

---

## 📚 Contents

| # | Notebook | Concept | What it demonstrates |
|---|----------|---------|----------------------|
| 01 | [`01_sequential_bmi_workflow.ipynb`](01_sequential_bmi_workflow.ipynb) | Sequential workflow | Basic `StateGraph`: nodes, edges, and state, using a BMI calculator |
| 02 | [`02_simple_llm_workflow.ipynb`](02_simple_llm_workflow.ipynb) | LLM in a graph | Calling an LLM from a graph node |
| 03 | [`03_prompt_chaining.ipynb`](03_prompt_chaining.ipynb) | Prompt chaining | Passing one LLM node's output as the next node's input |
| 04 | [`04_batsman_workflow.ipynb`](04_batsman_workflow.ipynb) | Multi-node state | Computing several derived metrics from a batsman's stats |
| 05 | [`05_Parallel_UPSC_essay_workflow.ipynb`](05_Parallel_UPSC_essay_workflow.ipynb) | Parallel workflow | Running multiple evaluation nodes in parallel and merging the results (UPSC essay evaluator) |
| 06 | [`06_contional_quadratic_equation_workflow.ipynb`](06_contional_quadratic_equation_workflow.ipynb) | Conditional edges | Routing based on state, using quadratic equation roots |
| 07 | [`07_conditional_llm_Based_workflow_review_reply_workflow.ipynb`](07_conditional_llm_Based_workflow_review_reply_workflow.ipynb) | LLM-based routing | Classifying a review's sentiment and routing to the right reply |
| 08 | [`08_loopWorkflow_X_post_generator.ipynb`](08_loopWorkflow_X_post_generator.ipynb) | Iterative loop | Generate, evaluate, and optimize loop for X (Twitter) posts |
| 09 | [`09_basic_chatbot.ipynb`](09_basic_chatbot.ipynb) | Chatbot | A basic conversational chatbot built with LangGraph |
| 10 | [`10_persistence.ipynb`](10_persistence.ipynb) | Persistence | Checkpointers and thread-based memory |
| 10 | [`10_persistence_indatabase.py`](10_persistence_indatabase.py) | Persistence (database) | Storing graph state in a database instead of memory |
| 14 | [`14_hitl.ipynb`](14_hitl.ipynb) | Human-in-the-loop | Pausing a graph for human input or approval before continuing |

---

## 🧠 Key Concepts Covered

- **State**: shared data (`TypedDict` / Pydantic) passed between nodes
- **Nodes and edges**: the building blocks of a workflow
- **Sequential, parallel, conditional, and looping** execution patterns
- **Prompt chaining** and **LLM-based decision making**
- **Persistence and memory** with checkpointers
- **Human-in-the-loop** interrupts

---

## 🚀 Getting Started

### Prerequisites

- Python 3.10+
- An API key for the LLM provider used in the notebooks (e.g. OpenAI or Google Gemini)
- Jupyter Notebook or JupyterLab (or VS Code with the Jupyter extension)

### Installation

```bash
# Clone the repository
git clone https://github.com/harshdethe/LangGraph.git
cd LangGraph

# Create and activate a virtual environment
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate

# Install dependencies
pip install langgraph langchain langchain-openai langchain-google-genai python-dotenv jupyter
```

> Install only the provider package you need (`langchain-openai` or `langchain-google-genai`).

### Environment variables

Create a `.env` file in the project root:

```env
OPENAI_API_KEY=your_openai_api_key
GOOGLE_API_KEY=your_gemini_api_key
```

### Run

```bash
jupyter notebook
```

Then open the notebooks in order, starting with `01_sequential_bmi_workflow.ipynb`.

---

## 🗂️ Project Structure

```
LangGraph/
├── 01_sequential_bmi_workflow.ipynb
├── 02_simple_llm_workflow.ipynb
├── 03_prompt_chaining.ipynb
├── 04_batsman_workflow.ipynb
├── 05_Parallel_UPSC_essay_workflow.ipynb
├── 06_contional_quadratic_equation_workflow.ipynb
├── 07_conditional_llm_Based_workflow_review_reply_workflow.ipynb
├── 08_loopWorkflow_X_post_generator.ipynb
├── 09_basic_chatbot.ipynb
├── 10_persistence.ipynb
├── 10_persistence_indatabase.py
├── 14_hitl.ipynb
└── README.md
```

---

## 🛠️ Tech Stack

- [LangGraph](https://github.com/langchain-ai/langgraph)
- [LangChain](https://github.com/langchain-ai/langchain)
- Python, Jupyter Notebook
- OpenAI / Google Gemini (LLM providers)

---

## 🗺️ Roadmap

- [ ] Tools and tool-calling agents
- [ ] ReAct agent
- [ ] Multi-agent workflows
- [ ] Subgraphs
- [ ] Streaming and observability (LangSmith)

---

## 🤝 Contributing

Suggestions and improvements are welcome. Feel free to open an issue or submit a pull request.

---

## 👤 Author

**Harsh Dethe**
GitHub: [@harshdethe](https://github.com/harshdethe)

---

⭐ If you find this repo useful, consider giving it a star!
