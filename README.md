## RealAI Prompt Optimizer + Executor

The **RealAI Prompt Optimizer + Executor** is a YAML-based prompt injection framework designed specifically for use with **Fundrise’s RealAI** environment. It enables users to append a structured instruction block directly after a natural language request so the model can:

1. Read and interpret the original user prompt  
2. Rewrite and optimize the prompt for clarity and execution quality  
3. Execute the task using the optimized version — automatically  

This creates a consistent, high-quality output workflow without requiring users to manually engineer perfect prompts.

---

## Why This Exists

Natural language prompts often contain ambiguity, missing structure, or unclear deliverable formats.  
This optimizer acts as a **self-improving prompt layer** that standardizes how RealAI interprets and executes requests.

Instead of relying on users to refine prompts through trial and error, the optimizer:

- Preserves original user intent  
- Clarifies constraints and success criteria  
- Removes ambiguity and unnecessary fluff  
- Converts requests into precise, executable instructions  
- Immediately performs the task using the improved prompt  

The result is faster, more reliable outputs with fewer iterations.

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
- Content creation (LinkedIn posts, internal briefs, etc.)  
- Workflow automation inside RealAI  
- Standardizing prompt quality across teams  
- Reducing iteration cycles with LLMs  

---

## How to Use

1. Write your request in natural language.
2. Paste the YAML optimizer block directly after your prompt.
3. Submit both together to RealAI.
4. The model will optimize and execute automatically.

No prompt engineering experience required.

---

## Design Philosophy

This optimizer is built on a simple principle:

**The user should only state what they want — the system handles how to execute it well.**

It functions as a reusable, portable prompt-quality layer that improves clarity, reliability, and usefulness across all RealAI sessions.
