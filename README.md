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
- **Auto Mode** → intelligent routing to the best mode  

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

# 🧠 Modes

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

## Auto Mode (Intelligent Router)
**Purpose:** Automatically select the best execution mode and run  

Auto Mode analyzes the user’s prompt and chooses between:
- Analyst Mode
- Research Mode

It then optimizes and executes immediately.

### When Auto Mode chooses Analyst
- Direct question  
- Metrics interpretation  
- Formatting-heavy requests  
- “Just answer” style prompts  
- Strict scope or output requirements  

### When Auto Mode chooses Research
- Strategy or implications requested  
- Market drivers or outlook requested  
- Investment framing or recommendations  
- Comparative analysis  
- Memo or narrative outputs  

### Why Auto Mode exists
Most users don’t want to decide which mode to use.

Auto Mode:
- Interprets prompt intent  
- Selects best execution style  
- Preserves constraints  
- Executes immediately  

Result:  
**Fast, decision-useful output with zero prompt engineering.**

---

# 🧰 Web Tool Mode Options

The web interface provides three selections:

**Analyst Mode**  
Direct execution using Analyst YAML.

**Research Mode**  
Direct execution using Research YAML.

**Auto Mode (Recommended)**  
Automatically selects best mode and executes.

When Auto Mode is selected, the web tool prepends:

MODE=AUTO

and appends the Auto Router YAML.

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

# Architecture

This repo contains:

- Analyst Mode YAML  
- Research Mode YAML  
- Auto Router YAML  
- Static web interface (index.html)  

The web interface dynamically loads YAML files and assembles the optimized prompt for easy copying into RealAI.

---

# Design Philosophy

**The user should only state what they want.  
The system determines how to execute it well.**

By separating:

- Analyst Mode → precision  
- Research Mode → insight  
- Auto Mode → intelligent routing  

…the framework becomes a reusable execution layer for RealAI.

It standardizes output quality, reduces prompt friction, and enables consistent institutional-grade analysis across sessions.
