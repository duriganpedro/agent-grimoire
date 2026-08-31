# agent-grimoire

Domain-specific autonomous agent specifications and skills grounded in canonical engineering literature.

---

## Architecture & Literature Foundations

The operational loop (Sense, Reason, Plan, Act, Coordinate) and guardrail topologies follow:

1. **Agentic Architectural Patterns for Building Multi-Agent Systems** (Ali Arsanjani, Juan Pablo Bustos)
2. **Building AI Agents with LLMs, RAG, and Knowledge Graphs** (Salvatore Raieli, Gabriele Iuculano)

---

## Agents

| Agent Name | Core Specialty | Foundational Doctrine |
| :--- | :--- | :--- |
| **`causal-inference`** | DAG modeling, ATE/CATE estimation & confounder control | *Causal Inference and Discovery in Python* (Aleksander Molak) |
| **`spatial-systems`** | PostGIS indexing, spatial SQL & geometric pipelines | *PostGIS in Action, 3rd Ed* (Regina Obe, Leo Hsu) |
| **`bayesian-modeling`** | Probabilistic programming, prior testing & MCMC diagnostics | *Bayesian Analysis with Python, 3rd Ed* (Osvaldo Martin) |
| **`refactoring`** | Code smell elimination & atomic transformations | *Refactoring: Improving the Design of Existing Code* (Martin Fowler, Kent Beck) |
| **`distributed-systems`** | Trade-off analysis, coupling metrics & data boundaries | *Software Architecture: The Hard Parts* (Neal Ford, Mark Richards) |
| **`systems-rust`** | Memory models, atomics & lock-free concurrency in Rust | *Rust Atomics and Locks* (Mara Bos) |
| **`software-testing`** | Systematic equivalence partitioning & mutation testing | *Effective Software Testing* (Mauricio Aniche) |

---

## Agent Directory Layout

```
agent-grimoire/
├── agents/             # Direct agent behavioral definitions (.md)
└── skills/             # Portable executable skills (SKILL.md)
    ├── causal-inference/
    ├── spatial-systems/
    ├── bayesian-modeling/
    ├── refactoring/
    ├── distributed-systems/
    ├── systems-rust/
    └── software-testing/
```

---

## Usage

### 1. Agent CLI / IDE Skills
Link or copy any skill into your project's `.agents/skills/` directory:

```bash
mkdir -p .agents/skills
cp -r /path/to/agent-grimoire/skills/spatial-systems .agents/skills/
```

### 2. Cursor / VS Code Agent Rules
Include the agent definition directly in your project root:

```bash
cp /path/to/agent-grimoire/agents/spatial-systems.md .cursorrules
```

### 3. Local Model Hosts (LM Studio / Ollama)
Import the agent specification into the model configuration preset or Modelfile.

---

## License
MIT License
