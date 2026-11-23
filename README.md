\# AI-Based Client Short Allocation and Shortfall Assistant



A Python-based project combining deterministic short allocation calculations with a local AI-powered assistant for understanding financial queries and explaining margin shortfalls.



\## Project Modules



\### Part 1A – Client Short Allocation Calculator

\- Accepts client details, market segment, peak margin and allocated collateral.

\- Calculates margin shortfall and applicable penalty slab.

\- Performs input validation and provides consistent results.

\- Uses deterministic calculation logic.



\### Part 1B – AI-Powered Shortfall Assistant

\- Understands natural-language financial queries.

\- Extracts client details and margin-related values.

\- Uses Ollama with the Qwen 2.5 (3B) model locally.

\- Validates extracted information and calculates shortfalls.

\- Provides explanations and requests clarification for missing information.



\## Tech Stack

\- Python

\- HTML, CSS, JavaScript

\- Ollama – Qwen 2.5 (3B)

\- Pytest, Ruff and Bandit



\## Run Locally



\*\*Part 1A\*\*



```powershell

cd part1a

python -m client\_short\_allocation.web

```



Open: `http://127.0.0.1:8000`



\*\*Part 1B\*\*



Start Ollama in a separate terminal:



```powershell

ollama run qwen2.5:3b

```



Run the application:



```powershell

cd part1b

python .\\src\\web.py --port 8001

```



Open: `http://127.0.0.1:8001`



\## Testing and Evaluation



\- Part 1A: 26 tests passed.

\- Part 1B: 35 tests passed.

\- Ruff: All checks passed.

\- Bandit: No security findings.

\- Part 1B evaluation: 15 cases passed with a 100% aggregate score.



\## Key Principles

\- Specification-Driven Development (SDD).

\- Local-first AI with no paid AI API dependency.

\- Deterministic financial calculations.

\- Input validation and transparent clarification handling.



\## Conclusion



The project demonstrates the combination of specification-driven engineering, reliable financial calculations and locally hosted AI to build an intelligent shortfall management solution.

