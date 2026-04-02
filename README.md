# Mindful Consumption Agent

A Claude Code agent prototype that helps people examine unnecessary wants driven by advertising and consumerism — and redirect toward genuine human flourishing.

## What It Does

Rather than shaming or lecturing, the agent uses **Socratic questioning**, **reframing**, and **gratitude-based reflection** to help users pause before impulse purchases and explore what they actually need.

### Skills

| Skill | Purpose |
|-------|---------|
| **Session Start** | Classifies user intent and routes to the right skill |
| **Want Examination** | Explores the deeper need behind a desire to buy |
| **Reframe** | Names persuasion techniques and suggests non-purchase alternatives |
| **Flourishing Prompt** | Offers scaled self-care exercises (1-10 min) for stress and low mood |
| **Gratitude Inventory** | Guides reflection on what already brings genuine satisfaction |

## Project Structure

```
data/
  personas/          # 4 simulated user personas (Maya, David, Priya, Jordan)
  interactions/      # Beneficial and unhelpful interaction examples
docs/
  process-guide.md   # Step-by-step prototyping walkthrough
  project-ideas.md   # 11 agent project ideas for students
eval/
  evaluate.py        # LLM-as-judge evaluation framework
  run_eval.py        # Runner (works without API keys)
experiments/         # Iteration logs and plans
```

## Context

Built as a live demo for **COS 598/498: Generative AI Agents** (Spring 2026, University of Maine). The repo serves as both a working prototype and a reference for students learning to prototype AI agents with Claude Code skills.