# 🕸️ LangGraph Practice

My personal practice files for learning [LangGraph](https://langchain-ai.github.io/langgraph/). This is not a single project. It is a collection of small notebooks I wrote while learning, going from basic graphs to LLM workflows, conditional routing, parallel execution, loops, chatbots, persistence, and human-in-the-loop (HITL).

Each file practices one concept and builds on the one before it.

---

## 📚 What I Practiced

| # | File | Concept | What it practices |
|---|------|---------|-------------------|
| 01 | [`01_sequential_bmi_workflow.ipynb`](01_sequential_bmi_workflow.ipynb) | Sequential workflow | Basic `StateGraph`: state, nodes, and edges (BMI calculator) |
| 02 | [`02_simple_llm_workflow.ipynb`](02_simple_llm_workflow.ipynb) | LLM in a graph | Calling an LLM from a graph node |
| 03 | [`03_prompt_chaining.ipynb`](03_prompt_chaining.ipynb) | Prompt chaining | Passing one LLM node's output into the next |
| 04 | [`04_batsman_workflow.ipynb`](04_batsman_workflow.ipynb) | Multi-node state | Calculating several metrics from a batsman's stats |
| 05 | [`05_Parallel_UPSC_essay_workflow.ipynb`](05_Parallel_UPSC_essay_workflow.ipynb) | Parallel workflow | Running nodes in parallel and merging results (UPSC essay evaluation) |
| 06 | [`06_contional_quadratic_equation_workflow.ipynb`](06_contional_quadratic_equation_workflow.ipynb) | Conditional edges | Routing based on state (quadratic equation) |
| 07 | [`07_conditional_llm_Based_workflow_review_reply_workflow.ipynb`](07_conditional_llm_Based_workflow_review_reply_workflow.ipynb) | LLM-based routing | Routing a review reply based on LLM output |
| 08 | [`08_loopWorkflow_X_post_generator.ipynb`](08_loopWorkflow_X_post_generator.ipynb) | Loop workflow | Generate, evaluate, and improve loop (X post generator) |
| 09 | [`09_basic_chatbot.ipynb`](09_basic_chatbot.ipynb) | Chatbot | A basic chatbot using LangGraph |
| 10 | [`10_persistence.ipynb`](10_persistence.ipynb) | Persistence | Checkpointers and thread-based memory |
| 10 | [`10_persistence_indatabase.py`](10_persistence_indatabase.py) | Persistence (DB) | Saving graph state in a database |
| 14 | [`14_hitl.ipynb`](14_hitl.ipynb) | Human-in-the-loop | Pausing a graph for human input before continuing |

---

## 🧠 Concepts Covered

- State, nodes, and edges
- Sequential, parallel, conditional, and loop workflows
- Prompt chaining and LLM-based routing
- Persistence and memory (checkpointers)
- Human-in-the-loop interrupts

---

## 🚀 How to Run

**Requirements:** Python 3.10+, Jupyter, and an API key for the LLM provider used in the notebooks.

```bash
git clone https://github.com/harshdethe/LangGraph.git
cd LangGraph

python -m venv venv
source venv/bin/activate        # Windows: venv\Scripts\activate

pip install langgraph langchain python-dotenv jupyter
# plus your LLM provider package, e.g.
# pip install langchain-openai   or   pip install langchain-google-genai
```

Create a `.env` file:

```env
OPENAI_API_KEY=your_key_here
GOOGLE_API_KEY=your_key_here
```

Then start Jupyter and open the notebooks in order:

```bash
jupyter notebook
```

---

## 🗺️ Still to Practice

- [ ] Tools and tool-calling agents
- [ ] ReAct agent
- [ ] Multi-agent workflows
- [ ] Subgraphs
- [ ] MCP with LangGraph

---

## 👤 Author

**Harsh Dethe** · [@harshdethe](https://github.com/harshdethe)

> These notebooks are for learning, so the code is kept simple and may not be production-ready.
