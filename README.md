## RealAI Prompt Optimizer Framework

The **RealAI Prompt Optimizer Framework** is a YAML-based prompt injection system designed specifically for use with **Fundrise’s RealAI** environment. It enables users to append a structured instruction block directly after a natural language request so the model can:

1. Read and interpret the original user prompt  
2. Rewrite and optimize the prompt for clarity and execution quality  
3. Execute the task using the optimized version — automatically  

This creates a consistent, high-quality output workflow without requiring users to manually engineer perfect prompts.

The framework includes **three distinct operating modes**:

- **Analyst Mode** → tight, scoped, execution-focused  
- **Research Mode** → contextual, insight-driven, investment-focused  
- **Mode Selector** → recommends and routes to the best mode before execution  

Together, they allow RealAI to function as a disciplined analyst, a strategic research desk, and an intelligent workflow router.

---

## 🚀 Live Web Tool (New)

A production-ready static web interface is now included.

Once GitHub Pages is enabled, you can use it here:  
**👉 https://domingos-s.github.io/RealAI-Prompt-Optimizer-Executor/**

### What it does
The web tool allows you to:

1. Paste your natural language prompt  
2. Select a mode (Analyst, Research, or Mode Selector)  
3. Click **Copy Combined Prompt**  
4. Paste directly into RealAI  

The page automatically:
- Pulls the latest YAML files from this repo  
- Appends the selected optimizer to your prompt  
- Copies the optimized prompt to your clipboard  
- Stays in sync with future YAML updates  

No manual YAML copying required.

---

## Repository Structure

This repository contains four core files:

- `RealAIPromptOptimizer-AnalystMode.yaml`  
- `RealAIPromptOptimizer-ResearchMode.yaml`  
- `RealAIPromptOptimizer-ModeSelector.yaml`  
- `index.html` (static web tool)

Each YAML file is self-contained and can be used independently.  
The web tool dynamically loads these YAML files directly from the repo.

---

## Why This Exists

Natural language prompts often contain ambiguity, missing structure, or unclear deliverable formats.  
This framework acts as a **self-improving prompt layer** that standardizes how RealAI interprets and executes requests.

Instead of relying on users to refine prompts through trial and error, the optimizer:

- Preserves original user intent  
- Clarifies constraints and success criteria  
- Removes ambiguity and unnecessary fluff  
- Converts requests into precise, executable instructions  
- Immediately performs the task using the improved prompt  

The result is faster, more reliable outputs with fewer iterations.

---

## Modes

### Analyst Mode
**Purpose:** Precision, discipline, and scoped execution.

Best for:
- Direct factual questions  
- Underwriting inputs  
- Operational metrics  
- Quick market checks  
- Repeatable workflows  
- When you want only what was asked — nothing extra  

Characteristics:
- Strict intent preservation  
- Minimal scope expansion  
- Concise, execution-first responses  
- Constraint-driven formatting  
- Highly predictable outputs  

Think: **Institutional analyst answering exactly the question asked.**

---

### Research Mode
**Purpose:** Insight, synthesis, and forward-looking intelligence.

Best for:
- Market research  
- Investment memos  
- Acquisition analysis  
- Strategy development  
- Thought leadership  
- Understanding implications, not just facts  

Characteristics:
- Answers the core question first  
- Expands into relevant context  
- Explains drivers and trends  
- Includes forward-looking implications  
- Frames insights for investors/operators  
- Research-desk level depth  

Think: **CRE research desk supporting investment decisions.**

---

### Mode Selector
**Purpose:** Intelligent routing between Analyst Mode and Research Mode.

Best for:
- When unsure which mode to use  
- Training new users or teams  
- Mixed analytical + strategic questions  
- New or exploratory workflows  

What it does:
- Interprets your prompt  
- Explains how each mode would approach it  
- Recommends the best mode  
- Lets you choose (or auto-select)  
- Executes using the selected mode  

Think: **Workflow router and execution advisor.**

---

## How to Use

### Fastest (Recommended)
Use the web tool:
1. Open the GitHub Pages link  
2. Paste your prompt  
3. Select mode  
4. Click **Copy Combined Prompt**  
5. Paste into RealAI  

### Manual Method
1. Write your prompt in natural language  
2. Copy the YAML for the desired mode  
3. Paste it after your prompt in RealAI  
4. Submit  

The optimizer will refine and execute automatically.

---

## Intended Use Cases

- Real estate and investment analysis  
- Underwriting support  
- Market research and memos  
- Investment committee preparation  
- Content creation and thought leadership  
- Workflow standardization across teams  
- Training analysts to use LLMs consistently  
- Reducing prompt iteration cycles  

---

## Design Philosophy

This framework is built on a simple principle:

**The user should only state what they want — the system determines how best to execute it.**

By separating **Analyst Mode**, **Research Mode**, and **Mode Selector**, users gain full control over output style:

- Precision when speed and clarity matter  
- Depth when insight and strategy matter  
- Guidance when unsure which approach fits  

The result is a reusable, portable prompt-quality layer that improves clarity, reliability, and usefulness across all RealAI sessions.