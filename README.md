# iQ

# LLM Deduction Engine (Akinator-Style Decision Tree)

A lightweight, high-performance, single-page interactive sandbox designed for mobile/iPad devices. It implements a deterministic decision-tree classification engine to deduce one of 25 curated Large Language Model (LLM) concepts based on system traits.

This repository serves as an educational tool for demonstrating taxonomic classification, binary feature space splitting, and interactive Web UI design.

## ✍️ Author & Credits

* **Game Concept & Premise:** Developed and conceptualized by [@sRowboat](https://github.com/sRowboat).
* **Technical Implementation:** Dynamic entropy-based path partitioning sandbox.

---

## 🚀 Architecture & Key Components

The application is structured entirely within a single self-contained HTML file (`llm_deduction_pro.html`), designed with **Vanilla JavaScript** and **Tailwind CSS**. It is divided into three logical layers:

### 1. The Taxonomic Lexicon (`lexicon`)

The application defines a curated database of 25 core LLM terms. Each term is represented as an object containing semantic descriptions alongside a boolean attribute vector across 6 taxonomic features:

```json
{ 
    "name": "Superposition", 
    "definition": "High-dimensional mathematical phenomenon where a model packs more features...",
    "is_structural": false, 
    "involves_training": false, 
    "data_unit": false, 
    "compute_saving": false, 
    "is_mathematical": true, 
    "is_phenomenon": true 
}
