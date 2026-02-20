# RealAI Prompt Optimizer Framework

The **RealAI Prompt Optimizer Framework** is a YAML-based prompt injection system designed specifically for use with **Fundrise’s RealAI** environment.

It allows users to append a structured optimizer block directly after a natural language request so the model can:

1. Interpret the original prompt  
2. Optimize it for clarity and execution quality  
3. Execute using the improved version automatically  

This creates a consistent, institutional-quality output workflow without requiring users to manually engineer perfect prompts.

The framework includes **three operating modes**:

- **Analyst Mode** → tight, scoped, execution-focused  
- **Research Mode** → contextual, insight-driven  
- **Mode Selector** → recommends or routes to the best mode  

Together, they allow RealAI to function as:
- A disciplined analyst  
- A strategic research desk  
- An intelligent workflow router  

---

# 🚀 Live Web Tool

👉 https://domingos-s.github.io/RealAI-Prompt-Optimizer-Executor/

A production-ready static interface is included in this repo.

### What it does
The web tool lets you:

1. Paste your natural language prompt  
2. Select a mode  
3. Click **Copy Combined Prompt**  
4. Paste directly into RealAI  

The page automatically:
- Pulls latest YAML files from this repo  
- Appends selected optimizer to your prompt  
- Copies combined prompt to clipboard  
- Stays synced with future YAML updates  

No manual YAML handling required.

---

# 🧠 Mode Selector (Updated Behavior)

Mode Selector now supports **interactive selection** and **auto-execution**.

### Interactive Mode Selector
When used without a mode token:

RealAI will:
1. Read the prompt  
2. Explain how Analyst vs Research would approach it  
3. Recommend a mode  
4. Ask the user to choose  
5. Pause execution  

User then replies with:

MODE=ANALYST  
MODE=RESEARCH  
MODE=AUTO  

Execution proceeds after selection.

### Auto Mode Selector
When MODE=AUTO is present:

- RealAI recommends a mode internally  
- Immediately executes  
- No pause or follow-up required  

### Why this exists
Some workflows require deliberate mode choice.  
Others require speed.

Mode Selector now supports both.

---

# 🧰 Web Tool Mode Options

The web interface provides four selections:

**Analyst Mode**  
Direct execution using Analyst YAML.

**Research Mode**  
Direct execution using Research YAML.

**Mode Selector (interactive)**  
RealAI explains modes and asks user to choose.

**Mode Selector (auto-execute)**  
Prepends MODE=AUTO and executes immediately.

An optional advanced override allows forcing:
- MODE=ANALYST  
- MODE=RESEARCH  
- MODE=AUTO  

---

# 📁 Repository Structure

RealAI-Prompt-Optimizer-Executor/
│
├── RealAIPromptOptimizer-AnalystMode.yaml  
├── RealAIPromptOptimizer-ResearchMode.yaml  
├── RealAIPromptOptimizer-ModeSelector.yaml  
├── index.html   (live web tool)  
└── README.md  

Each YAML file is fully self-contained and usable independently.  
The web tool dynamically pulls them from GitHub via raw URLs.

---

# Why This Exists

Natural language prompts often contain:
- Ambiguity  
- Missing structure  
- Unclear deliverables  

This framework acts as a **prompt quality layer** that standardizes execution inside RealAI.

Instead of iterative prompt tweaking, it:

- Preserves intent  
- Clarifies constraints  
- Defines success criteria  
- Removes fluff  
- Converts requests into executable instructions  
- Executes immediately  

Result:  
**Faster, more reliable, institutional-grade outputs.**

---

# Modes

## Analyst Mode
**Purpose:** Precision and scoped execution  

Best for:
- Direct factual questions  
- Underwriting inputs  
- Operational metrics  
- Quick market checks  
- Repeatable workflows  

Characteristics:
- Strict intent preservation  
- Minimal scope expansion  
- Concise outputs  
- Constraint-first logic  
- Highly predictable  

Think:  
**Institutional analyst answering exactly what was asked.**

---

## Research Mode
**Purpose:** Insight and forward-looking intelligence  

Best for:
- Market research  
- Investment memos  
- Acquisition analysis  
- Strategy development  
- Thought leadership  

Characteristics:
- Answers core question first  
- Adds relevant context  
- Explains drivers  
- Provides implications  
- Investor/operator framing  

Think:  
**CRE research desk supporting investment decisions.**

---

## Mode Selector
**Purpose:** Intelligent routing + execution control  

Best for:
- Unsure which mode fits  
- Training teams  
- Mixed analytical/strategic questions  
- New workflows  

Capabilities:
- Interprets prompt  
- Explains both approaches  
- Recommends mode  
- Allows user selection  
- Executes after selection or auto  

Think:  
**Workflow router for RealAI.**

---

# How to Use

## Fastest (Recommended)
Use the web tool:

1. Open GitHub Pages link  
2. Paste prompt  
3. Select mode  
4. Click Copy Combined Prompt  
5. Paste into RealAI  

## Manual Method
1. Write prompt  
2. Copy desired YAML  
3. Paste below prompt  
4. Submit in RealAI  

---

# Intended Use Cases

- Real estate and investment analysis  
- Underwriting workflows  
- Market research  
- IC memo prep  
- Thought leadership  
- Team prompt standardization  
- LLM workflow training  
- Reducing iteration cycles  

---

# Design Philosophy

**The user should only state what they want.  
The system determines how to execute it well.**

By separating:

- Analyst Mode → precision  
- Research Mode → insight  
- Mode Selector → guidance  

…the framework becomes a reusable execution layer for RealAI.

It standardizes output quality, reduces prompt friction, and enables consistent institutional-grade analysis across sessions.
