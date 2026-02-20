## RealAI Prompt Optimizer Framework

The **RealAI Prompt Optimizer Framework** is a YAML-based prompt injection system designed specifically for use with **Fundrise’s RealAI** environment. It enables users to append a structured instruction block directly after a natural language request so the model can:

1. Read and interpret the original user prompt  
2. Rewrite and optimize the prompt for clarity and execution quality  
3. Execute the task using the optimized version — automatically  

This creates a consistent, high-quality output workflow without requiring users to manually engineer perfect prompts.

The framework includes **two distinct operating modes**:

- **Analyst Mode** → tight, scoped, execution-focused  
- **Research Mode** → contextual, insight-driven, investment-focused  

Together, they allow RealAI to function as both a disciplined analyst and a strategic research desk.

---

## Repository Structure

This repository contains two independent YAML configuration files:

- `RealAIPromptOptimizer-AnalystMode.yaml`  
- `RealAIPromptOptimizer-ResearchMode.yaml`  

Each file is self-contained and can be used independently.  
There is no internal switching logic — users choose the mode explicitly by pasting the corresponding YAML block after their natural language prompt.

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

## Key Capabilities

### Intent Preservation
Captures the user’s true objective, audience, tone, and constraints before rewriting anything.

### Prompt Rewriting + Optimization
Transforms unstructured or loosely defined requests into clear, execution-ready prompts tailored for RealAI performance.

### Automatic Execution
After optimization, the model immediately acts on the improved prompt — no additional user input required.

### Constraint-First Logic
User formatting, tone, and structural requirements are treated as **hard rules** and always take priority.

### Assumption Handling
If inputs are missing but non-critical:
- Minimal, transparent assumptions are made  
- Execution proceeds  

If critical inputs are missing:
- The model asks only the most necessary clarifying questions  

### Structured Outputs
Ensures consistent response sections:
- **Understanding**  
- **Optimized Prompt**  
- **Output (final result)**  

---

## Intended Use Cases

- Real estate and investment analysis prompts  
- Underwriting and financial modeling support  
- Market research and memos  
- Investment committee preparation  
- Content creation (LinkedIn posts, internal briefs, etc.)  
- Workflow automation inside RealAI  
- Standardizing prompt quality across teams  
- Reducing iteration cycles with LLMs  

---

## How to Use

1. Write your request in natural language.  
2. Choose a mode:
   - Use **Analyst Mode** for tight, scoped answers  
   - Use **Research Mode** for deeper insight and context  
3. Paste the selected YAML optimizer block directly after your prompt.  
4. Submit both together to RealAI.  
5. The model will optimize and execute automatically.

No prompt engineering experience required.

---

## Design Philosophy

This framework is built on a simple principle:

**The user should only state what they want — the system determines how deeply to analyze it.**

By separating **Analyst Mode** and **Research Mode**, users gain control over output style:

- Precision when speed and clarity matter  
- Depth when insight and strategy matter  

The result is a reusable, portable prompt-quality layer that improves clarity, reliability, and usefulness across all RealAI sessions.
