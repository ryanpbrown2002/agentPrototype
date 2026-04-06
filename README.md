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

## How to Run

### Prerequisites

1. Install [Claude Code](https://docs.anthropic.com/en/docs/claude-code):
   - **Terminal (CLI):** Follow the [install guide](https://docs.anthropic.com/en/docs/claude-code)
   - **VS Code / Cursor:** Install the **Claude Code** extension from the extensions marketplace, then open the Claude Code panel from the sidebar
2. Clone this repository:
   ```bash
   git clone <repo-url>
   cd s26_3_31_class_and_guide-main
   ```
3. Open the project in Claude Code:
   - **Terminal:** Run `claude` from the project directory
   - **VS Code / Cursor:** Open the project folder, then open the Claude Code panel — it will automatically use the project directory

### Using the Agent

Once Claude Code is running in this project directory, the career agent skills are automatically available.

**To get started, type `/session-start` in the Claude Code chat.** This will classify your intent and route you to the right career skill. From there, just describe what you need help with — the agent will guide you through the rest.

#### Example Prompts

Try starting with `/session-start` and then following up with requests like these:

- "I'm a junior in college majoring in computer science and I'm looking for summer internships. Can you help me get started?"
- "Help me find entry-level marketing jobs in the Portland, Maine area."
- "Review my resume and suggest improvements for applying to data analyst positions." *(paste or attach your resume)*
- "Walk me through how to apply for a job I found on LinkedIn."
- "Screen this job posting for any concerns I should know about before applying." *(paste the job listing)*
- "Help me practice for a behavioral interview at a nonprofit organization."

#### Slash Commands

You can also invoke individual skills directly at any time:

| Command | What it does |
|---------|-------------|
| `/session-start` | **Start here** — classifies your intent and routes to the right skill |
| `/job-search` | Find relevant job listings |
| `/resume-review` | Get feedback on your resume or cover letter |
| `/application-guide` | Step-by-step help with applying |
| `/job-screening` | Flag concerns about a specific job posting |
| `/interview-prep` | Practice interview questions in a safe space |

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
