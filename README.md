# CARE-iESO-Agent

CARE-iESO-Agent is a structured repository for documenting and applying the **CARE (Collaborative Agent Reasoning Engineering)** methodology to design a reliable **IESO-style** LLM chatbot agent for **NASA Worldview**:
[https://worldview.earthdata.nasa.gov/](https://worldview.earthdata.nasa.gov/)

This repository captures **structured design documentation and reusable artifacts** for building an agent that helps users interpret, explore, and validate Earth observation imagery and related dataset context inside NASA Worldview—while staying grounded in authoritative sources and SME-reviewed behaviors.

---

## Project Focus: IESO Agent for NASA Worldview
This work is specifically tailored to an **iESO/Worldview design pattern**, where the agent operates through a consistent engineering loop. The goal is to produce a **reviewable, testable agent design** that supports both new and expert users in performing correct scientific and operational interpretation of what they see in NASA Worldview.

---

## Participating SMEs

This project will be developed collaboratively with participating subject-matter experts:
* **Rousseaux, Cecile S. (GSFC-6160)** — [ian.g.brosnan@nasa.gov](mailto:cecile.s.rousseaux@nasa.gov)
* **Brosnan, Ian G. (ARC-SG)** — [ian.g.brosnan@nasa.gov](mailto:ian.g.brosnan@nasa.gov)
* **Hain, Christopher R. (MSFC-ST11)** — [christopher.hain@nasa.gov](mailto:christopher.hain@nasa.gov)
* **Cetinic, Ivona (GSFC-616.0) [MORGAN STATE UNIV.]** — [ivona.cetinic@nasa.gov](mailto:ivona.cetinic@nasa.gov)
* **Felikson, Denis (GSFC-6150)** — [denis.felikson@nasa.gov](mailto:denis.felikson@nasa.gov)
* **Kumar, Sujay V (GSFC-6170)** — [sujay.v.kumar@nasa.gov](mailto:sujay.v.kumar@nasa.gov)

---

## What is CARE?

**CARE (Collaborative Agent Reasoning Engineering)** is a staged, artifact-driven methodology for engineering LLM agents that are:

* Explicitly specified rather than prompt-tuned by trial and error
* Grounded in authoritative Earth science and NASA/Earthdata context
* Designed with transparent reasoning policies and guardrails
* Evaluated with realistic queries and structured benchmarks

CARE emphasizes **repeatability, reviewability, and maintainability** of agent behavior over time, enabling safe iteration as datasets, UI behavior, and science expectations evolve.

---

## Repository Purpose

This repository exists to:
* Organize CARE artifacts specifically for the **NASA Worldview chatbot agent**
* Capture **IESO phase prompts**, specifications, and outputs in a reviewable format
* Support collaboration between SMEs, developers, and LLM-based helper agents
* Track design evolution, decisions, and benchmarking results over time

The focus is primarily on **agent design documentation and evaluation artifacts**, not runtime application code.

---

## CARE Phases (IESO-Aligned)

The repository is organized into five CARE phases, mapped to IESO design needs:

### **Phase 1: Scope and Decompose (Interpret)**

Define user goals, scientific intent classes, constraints, and operational boundaries in Worldview.

### **Phase 2: Key Information Elicitation (Explore)**

Document datasets, layer metadata, authoritative references, known pitfalls, and required context.

### **Phase 3: Reasoning Policy and Guardrails (Interpret + Synthesize)**

Define verification rules, uncertainty handling, citation expectations, and safety/failure behaviors.

### **Phase 4: Prompt Architecture and Tool Orchestration (Explore + Operationalize)**

Translate the design into structured prompts, tool routing, UI action steps, and response templates.

### **Phase 5: Benchmarking (Synthesize + Operationalize)**

Build scenario-based test suites (scientific + operational), rubrics, and regression evaluation outputs.

---

## Repository Structure

```text
AKD-CARE/
├── phase_1_scope_and_decompose/
├── phase_2_key_information_elicitation/
├── phase_3_reasoning_policy_and_guardrails/
├── phase_4_prompt_architecture_and_tool_orchestration/
├── phase_5_benchmarking/
├── examples/
├── docs/
└── changelog.md
```

---

## Outcome

The deliverable of this repo is a **reusable, reviewable IESO agent design package** for NASA Worldview—supporting:

* user intent understanding (scientific + operational)
* grounded assistance for selecting imagery/layers/time ranges
* careful interpretation aligned with Earth science best practices
* actionable guidance for using Worldview correctly
* evaluation that goes beyond demos into repeatable benchmarks
