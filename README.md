# Cintia Millan

AI/LLM engineer based between Lisbon and Sao Paulo, currently at Web Summit. Interested in agent architectures, tool use, and the applied-RL side of getting models to act reliably, not just talk well.

## A few things I've built

- **[summit_agent](https://github.com/CiMillan/summit_agent)** — a Ruby framework for tool-using LLM agents, built around a bounded ReAct loop, with a real local-LLM backend (Ollama, tool-calling) — not a mock. Building the real adapter surfaced a bug no stub could have: the agent never recorded its own tool-call turn in conversation history, so a real model just re-asked for the tool forever. The README's "Design Decisions" section walks through that and four other trade-offs — what I'd change next, and why each one is a trade-off rather than a mistake.
- **[MAS-IL-RL](https://github.com/CiMillan/MAS-IL-RL)** — a multi-agent simulation replicating a *Scientific Reports* paper on the coexistence of imitation learning and reinforcement learning in cooperation evolution.
- **[stacking-game-academic](https://github.com/CiMillan/stacking-game-academic)** — a game-theoretic model of Proof-of-Stake validator concentration: risk-adjusted equilibrium analysis with Monte Carlo simulation, calibrated against Ethereum and Cosmos.
- **[crypto-vol-quickstart](https://github.com/CiMillan/crypto-vol-quickstart)** — a volatility forecasting scaffold comparing GARCH, XGBoost, and LSTM models with walk-forward validation.

I try to document *why* a project is built the way it is, not just what it does — the README of whatever's pinned above is usually the best place to see how I think through a design trade-off.
