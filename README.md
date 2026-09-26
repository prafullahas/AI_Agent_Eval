# AI_Agent_Eval

## Multi-Dimensional AI Agent Evaluation & Failure Analysis Framework

AgentEval+ is a practical framework for evaluating and comparing AI agents across multiple dimensions of task performance.

The project extends a CQ Math-style agent evaluation workflow into a multi-agent evaluation pipeline with automated scoring, matched-task comparison, statistical analysis, failure analysis, and exportable results.

The framework evaluates agents on:

- Correctness
- Reasoning Quality
- Instruction Following
- Relevance
- Clarity

It also provides task-level, category-level, and agent-level analysis to help identify where AI agents succeed and where they fail.

---

## Features

- Multi-agent evaluation
- Mathematical reasoning benchmark
- Multiple evaluation dimensions
- Automated baseline scoring
- Gemini-based AI agent integration
- Matched-task comparison
- Category-level analysis
- Failure detection
- Failure-mode analysis
- Statistical analysis
- Confidence interval analysis
- Per-task comparison
- Data visualization
- CSV result exports
- JSON evaluation report
- Reproducible notebook workflow

---
**# Limitations**

Small benchmark size
Heuristic baseline evaluation
API availability and quota limitations
Primarily focused on mathematical reasoning
Simplified evaluation criteria

**# Future Improvements**

Larger benchmarks
LLM-as-a-Judge
Independent judge models
Pairwise agent evaluation
Advanced failure classification
Human evaluation
Agent trajectory evaluation
Tool-use evaluation
Cost and latency benchmarking
Interactive Streamlit dashboard
Automated experiment tracking

**#Tech Stack**

Python
Jupyter
Microsoft AutoGen
Gemini API
Pandas
NumPy
Scikit-learn
Matplotlib

---
## Project Architecture

```text
                    ┌──────────────────────┐
                    │    Benchmark Tasks   │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │     AI Agents        │
                    │                      │
                    │  Agent A             │
                    │  Agent B             │
                    │  Gemini              │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │   Agent Responses    │
                    └──────────┬───────────┘
                               │
                               ▼
              ┌──────────────────────────────────┐
              │       Evaluation Pipeline        │
              │                                  │
              │  Correctness                     │
              │  Reasoning Quality               │
              │  Instruction Following           │
              │  Relevance                       │
              │  Clarity                         │
              └────────────────┬─────────────────┘
                               │
                               ▼
              ┌──────────────────────────────────┐
              │      Analysis & Comparison       │
              │                                  │
              │  Agent Comparison                │
              │  Category Analysis               │
              │  Matched Tasks                   │
              │  Failure Analysis                │
              │  Statistics                      │
              └────────────────┬─────────────────┘
                               │
                               ▼
              ┌──────────────────────────────────┐
              │        Results & Reports         │
              │                                  │
              │  CSV                             │
              │  JSON                            │
              │  Visualizations                  │
              └──────────────────────────────────┘



