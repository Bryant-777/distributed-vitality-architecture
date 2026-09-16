# SUPPLEMENTAL_README.md
## Distributed Vitality Architecture (DVA) — Multi-Agent Extension (v3)

This supplement outlines the operational framework for migrating the core kernel into a decentralized, multi-agent topology. In alignment with anti-Goodhart design principles, this architecture strictly avoids centralized control assumptions and globally rigid metrics. Global System Vitality (V) remains an emergent property, driven by independent nodes managing localized trajectory vectors.

---

### 1. The Core Objective: Non-Irreversibility
The primary mandate of the Distributed Vitality Architecture is the preservation of future high-quality trajectories. System failure is defined not by localized conflict or data noise (Δ), but by **irreversibility**—the permanent collapse of viable future states and optionality.

---

### 2. The Local Proxy Engine (Signal Framework)
Rather than executing a hardcoded global equation, individual agents evaluate incoming token paths locally using an array of proxy signals. These signals assess the structural geometry of the trajectory manifold:

*   **N (Semantic Variance):** Measures the raw exploration capacity of the current state space.
*   **C_{local} (Local Compression):** Detects immediate, stagnant, or repetitive loops.
*   **C_{global} (Global Drift):** Detects unintended macro-drift away from the established trajectory manifold.
*   **P (Path Confidence):** Monitors for systemic "lock-in" or dangerous over-certainty.
*   **D (Directional Coherence):** Verifies semantic consistency, acting as a filter to separate constructive divergence from random noise.
*   **G (Meaning Gain):** Tracks long-range information density and conceptual expansion.

#### Local Viability Computation (ϕ)
Each autonomous agent represents an isolated trajectory cluster with its own unique α (evaluation weights). Agents dynamically calculate local path viability (ϕ) using normalized weights (w_*) to prevent single-signal domination:

ϕ = (w_N * N + w_D * D + w_G * G) - (w_C * C_{local} + w_P * P)

---

### 3. Temporal Smoothing & The Valley Crossing Rule
To protect the system from prematurely truncating high-potential paths that look temporarily chaotic, agents must calculate a smoothed directional trend over a historical window of k steps:

Trend = mean(Δϕ over last k steps)

*   **The Golden Rule:** If Trend > 0, the path **MUST NOT** be interrupted.
*   This protects **"Valley Crossing"**—temporary drops in baseline viability that naturally precede structural breakthroughs and non-linear growth trajectories.

---

### 4. Control Logic & Guided Divergence
A localized Soft Reset or regulatory intervention is triggered if, and only if, the following two conditions are simultaneously met:

1.  Trend ≤ 0 AND Meaning Gain (G) is low relative to the recent baseline.
2.  Stagnation signals are critically high (indicated by low compression or hyper-elevated Path Confidence).

#### Graded Response Protocol
Upon trigger activation, the node executes a two-tier response rather than a binary rejection:
*   **Tier 1:** Incrementally scale temperature (T) by 0.1–0.2 and apply mild repetition penalties to break the immediate loop.
*   **Tier 2 (Guided Divergence):** Sample alternative path candidates, intentionally biasing selection toward candidates with highly diverse ϕ scores across the set to force directed exploration over random noise.

---

### 5. Preservation of the Nutrient Buffer
To maintain systemic resilience against blind spots, the network mandates that **30% of the sampling population remain uniform and unmoderated**. This Nutrient Buffer preserves low-probability paths that may yield immense future value currently invisible to the active regulators.

---

### 6. Multi-Agent Entry Orientations
When initializing new peer nodes within the manifold, the following runtime constraints are permanently preloaded:
*   Evaluate forward-looking trajectories, never static outputs.
*   Treat structural perturbation (Δ) as a necessary shaping force, not an error to eliminate.
*   Maintain individual node calibration thresholds recursively to keep the shared immune system fully visible and reversible.
