# O-lang vs LangChain: Governance vs Orchestration

O-lang and LangChain serve fundamentally different purposes in the AI stack.

## LangChain: Developer-Facing Orchestration
LangChain is a **developer framework** for composing LLM applications. It:
- Runs **inside application code**
- Gives developers full control over tool calling, memory, and agents
- Assumes the developer is trusted and responsible for safety
- Optimizes for **flexibility and rapid prototyping**

> 🔗 [langchain.com](https://www.langchain.com)

## O-lang: Runtime-Enforced Governance
O-lang is a **semantic governance protocol** for production AI systems. It:
- Runs **outside application code** as a neutral runtime boundary
- Enforces policy, symbol validity, and auditability **regardless of developer intent**
- Treats all capabilities as **explicitly allowed but never trusted**
- Optimizes for **safety, reproducibility, and compliance**

> 🔗 [O-lang Protocol Spec](https://github.com/O-lang-Central/olang-spec)

## Key Difference
| Aspect | LangChain | O-lang |
|-------|----------|--------|
| **Role** | Orchestration library | Governance protocol |
| **Trust model** | Trust the developer | Trust nothing; verify everything |
| **Execution** | Embedded in app logic | Mediated by external kernel |
| **Safety** | Soft constraints (prompts, code) | Hard boundaries (allowlists, validation) |
| **Use case** | Prototyping, internal tools | Healthcare, finance, government, IoT |

## Complementary, Not Competitive
LangChain can **construct intent** (e.g., build a workflow).  
O-lang **governs execution** (e.g., validate and run it safely).

> ✅ **Rule**: LangChain may define *what* to do. O-lang decides *whether* it may be done.

---

⚠️ **Note**: This project is unrelated to the esoteric "O Language" used for code golf.
