# Cintia Millan

PhD researcher at NOVA IMS (Lisbon), working on multi-agent systems, evolutionary game theory, and the fragility of cooperation in hybrid human–AI populations — when the mechanisms that sustain cooperation (reputation, punishment, network structure) hold up as agents shift from human-supervised to autonomous, reward-driven adaptation, and when they quietly break. At Web Summit, I lead how LLM agents get integrated into our infrastructure — not as a novelty layer bolted on top, but as systems that have to integrate cleanly, fail predictably, and be trusted the same way any other production system is.

## Research

- **[multi-agent-system-RL](https://github.com/CiMillan/multi-agent-system-RL)** — agent-based simulation replicating a *Scientific Reports* paper (Tang, Wang & Xing, 2025) on the coexistence of imitation learning and reinforcement learning in cooperation evolution. Checked against the paper's reported results and fixed three bugs in my own implementation along the way — well-mixed populations now match closely, square-lattice mostly matches with one open discrepancy documented in the README.
- **[pos-validator-game](https://github.com/CiMillan/pos-validator-game)** — game-theoretic model of Proof-of-Stake validator concentration: risk-adjusted equilibrium analysis with Monte Carlo simulation, calibrated against Ethereum and Cosmos.

## Also building

- **[summit_agent](https://github.com/CiMillan/summit_agent)** — a Ruby framework for tool-using LLM agents, built around a bounded ReAct loop, with a real local-LLM backend (Ollama, tool-calling) — not a mock. Wiring up the real backend is what surfaced it: the agent recorded a tool's result in conversation history but never its own request for that tool, so a real model — reasoning over that history each turn — had no way to know it had already asked, and looped forever. The README's "Design Decisions" section walks through that and four other trade-offs.
- **[volatility-forecast](https://github.com/CiMillan/volatility-forecast)** — a volatility forecasting scaffold comparing GARCH, XGBoost, and LSTM models with walk-forward validation.

---

I try to document *why* a project is built the way it is, not just what it does — the README of whatever's pinned above is usually the best place to see how I think through a design trade-off.
