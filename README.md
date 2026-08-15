# Cintia Millan

Growth engineer based between Lisbon and São Paulo, currently at Web Summit, where I build and maintain the data infrastructure connecting our growth stack — Salesforce, Monday.com, Metabase — into a Presto/Trino-backed warehouse. Lately focused on where LLM agents fit into that kind of infrastructure: not as a novelty layer, but as another system that has to integrate cleanly, fail predictably, and be debuggable when something breaks.

## Experience

- **Web Summit — Growth Engineering.** Core contributor to the team's internal data infrastructure: ETL and integrations across Salesforce, Monday.com, and Metabase, feeding a Presto/Trino warehouse used for growth reporting.

## A few things I've built

- **[summit_agent](https://github.com/CiMillan/summit_agent)** — a Ruby framework for tool-using LLM agents, built around a bounded ReAct loop, with a real local-LLM backend (Ollama, tool-calling) — not a mock. Wiring up the real backend is what surfaced it: the agent recorded a tool's result in conversation history but never its own request for that tool, so a real model — reasoning over that history each turn — had no way to know it had already asked, and looped forever. The README's "Design Decisions" section walks through that and four other trade-offs — what I'd change next, and why each one is a trade-off rather than a mistake.
- **[multi-agent-system-RL](https://github.com/CiMillan/multi-agent-system-RL)** — a multi-agent simulation replicating a *Scientific Reports* paper on the coexistence of imitation learning and reinforcement learning in cooperation evolution.
- **[pos-validator-game](https://github.com/CiMillan/pos-validator-game)** — a game-theoretic model of Proof-of-Stake validator concentration: risk-adjusted equilibrium analysis with Monte Carlo simulation, calibrated against Ethereum and Cosmos.
- **[volatility-forecast](https://github.com/CiMillan/volatility-forecast)** — a volatility forecasting scaffold comparing GARCH, XGBoost, and LSTM models with walk-forward validation.

I try to document *why* a project is built the way it is, not just what it does — the README of whatever's pinned above is usually the best place to see how I think through a design trade-off.
