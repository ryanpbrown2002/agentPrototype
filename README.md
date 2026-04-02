# Ethical Career Agent

A Claude Code agent prototype that helps people navigate job searching, resume building, applications, and career decisions with honesty, encouragement, and ethical transparency.

## Who It's For

- **Internship seekers** getting their first professional experience
- **Post-graduates** entering the job market
- **Career changers** new to a field
- **Anyone** who wants a supportive, judgment-free career guide

## What It Does

The agent addresses the gap many people face when seeking work online -- the typical means of applying for jobs today. It provides relevant job suggestions, helps update resumes, walks users through the application process, and proactively flags important details that could affect their experience (disqualifications, drug testing, mandatory qualifications, disability accommodations, and potential moral/ethical concerns with positions).

A successful interaction looks like:

> **User:** "I'm looking for jobs in marketing, and I need help updating my resume to apply."
>
> **Agent:** Provides relevant listings, suggests resume updates tailored to marketing roles, explains how to apply, encourages the user realistically, and flags any important details about positions -- like required certifications, drug testing policies, or known controversies -- so the user can make informed decisions.

The agent is **encouraging but realistic**, and creates a space where users feel comfortable asking questions they might be nervous to ask a real interviewer.

### Skills

| Skill | Purpose |
|-------|---------|
| **Session Start** | Classifies user intent and routes to the right career skill |
| **Job Search** | Helps find relevant listings based on field, experience, and interests |
| **Resume Review** | Reviews and suggests updates to resumes, CVs, and cover letters |
| **Application Guide** | Walks users through how to apply, what to expect, and how to follow up |
| **Job Screening** | Ethically flags potential concerns -- disqualifications, drug testing, controversies, accommodations |
| **Interview Prep** | Safe space to practice interviews and ask sensitive questions without judgment |

## Project Structure

```
data/
  personas/          # Simulated user personas
  interactions/      # Beneficial and unhelpful interaction examples
docs/
  process-guide.md   # Step-by-step prototyping walkthrough
  project-ideas.md   # Agent project ideas for students
eval/
  evaluate.py        # LLM-as-judge evaluation framework
  run_eval.py        # Runner (works without API keys)
experiments/         # Iteration logs and plans
```

## Context

Built as a project for **COS 598/498: Generative AI Agents** (Spring 2026, University of Maine). The repo serves as both a working prototype and a reference for students learning to prototype AI agents with Claude Code skills.
