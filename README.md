<div align="center">

# 🚦 NeuroTraffic-RL

**Research-Grade Intelligent Traffic Signal Control Systems via Deep Reinforcement Learning**

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/release/python-3100/)
[![SUMO 1.18.0+](https://img.shields.io/badge/SUMO-1.18.0+-green.svg)](https://sumo.dlr.de/docs/Downloads.php)
[![Stable Baselines3](https://img.shields.io/badge/RL-Stable%20Baselines3-purple.svg)](https://stable-baselines3.readthedocs.io/en/master/)
[![Gymnasium](https://img.shields.io/badge/Environment-Gymnasium-orange.svg)](https://gymnasium.farama.org/)

</div>---

NeuroTraffic-RL is a clean, robust, and extensible reinforcement learning pipeline designed to optimize traffic signal control. Built on top of the world-class SUMO traffic simulator, it allows AI agents to learn optimal control policies to minimize congestion, reduce waiting times, and maximize throughput.

Currently in **Phase 1**, the system implements a highly optimized Proximal Policy Optimization (PPO) agent controlling a single complex 4-way intersection (Casablanca), beating fixed-cycle baselines.

---

## ✨ Key Features (Phase 1)

*   **Clean Architecture:** Strict separation of concerns. SUMO logic, Gym environments, RL agents, and visualizations are entirely decoupled.
*   **State-of-the-Art RL:** Native integration with Gymnasium and Stable-Baselines3 (PPO).
*   **Intelligent State Representation:** 26-dimensional feature vector per intersection combining queue lengths, densities, wait times, and temporal data.
*   **Custom Reward Shaping:** Configurable 4-component reward function balancing wait times, throughput, starvation, and phase-oscillation penalties.
*   **Real-time Dashboard:** A live Streamlit dashboard tracking KPIs (Queue Lengths, Waiting Time, Phases) during training and evaluation.
*   **Headless & GUI Modes:** Train blindingly fast in the background, or watch the agent learn in the SUMO GUI.

---
