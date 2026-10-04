# Claude Feature Set

This repository is a personal learning workspace for preparing for the Claude Certified Architect – Foundations certification.

The goal is to capture the key concepts, architecture patterns, and practical study notes needed to prepare for this exam in one place.

## Exam reference

- Official PDF: https://everpath-course-content.s3-accelerate.amazonaws.com/instructor%2F6nizmqk8tpzpfjvt6qmmav7rh%2Fpublic%2F1783542750%2FClaude+Certified+Architect+%E2%80%93+Foundations+Exam+Guide.pdf
- This repo consolidates the key exam details and study guidance based on the exam guide and related public certification material.

## Claude Certified Architect – Foundations overview

This certification is intended for people designing and implementing real-world solutions with Anthropic's Claude platform, especially around:

- Claude Code
- Claude API and application integration
- Agent orchestration and tool use
- Model Context Protocol (MCP)
- Production reliability, context management, and prompt design

## Exam at a glance

- Format: 60 multiple-choice, scenario-based questions
- Duration: 120 minutes
- Passing score: 720/1000
- Delivery: Proctored exam
- Price: $125 per attempt
- Validity: 12 months
- Audience: Solution architects, software engineers, and AI practitioners building with Claude

## Exam domains and weightings

### 1) Agentic Architecture & Orchestration (27%)
Focus on:

- Multi-agent system design
- Task decomposition and coordination patterns
- Tool invocation and delegation strategies
- Error handling and escalation between agents
- Preventing loops, dead ends, and brittle workflows

Study focus:

- When to use a single agent vs. orchestrated agent team
- Designing feedback loops that are controllable and observable
- Determining where tool calling or structured workflows should be used instead of free-form prompting

### 2) Claude Code Configuration & Workflows (20%)
Focus on:

- CLAUDE.md and repo-level AI workflow instructions
- Custom commands and repeatable developer workflows
- CI/CD integration for AI-assisted engineering
- Practical patterns for using Claude Code in real teams

Study focus:

- How to structure project context for effective Claude usage
- How to encode workflow rules in a maintainable way
- How to integrate Claude into engineering processes without creating operational risk

### 3) Prompt Engineering & Structured Output (20%)
Focus on:

- Few-shot prompting and pattern design
- Input validation and retry loops
- Structured output contracts and formatting
- Getting deterministic, production-safe model behavior

Study focus:

- When prompt design is sufficient versus when code or validation logic is required
- Controlling output format reliably
- Designing robust guardrails around responses

### 4) Tool Design & MCP Integration (18%)
Focus on:

- Designing effective tool descriptions for LLM selection
- MCP server architecture and integration patterns
- Tool reliability, structured results, and failure signaling
- Planning for production integrations and operational observability

Study focus:

- Use of MCP to expose tools and context cleanly
- Error structures such as isError and isRetryable
- Ensuring the model can choose the right tool under imperfect conditions

### 5) Context Management & Reliability (15%)
Focus on:

- Context window optimization
- Filtering and summarization strategies
- Information provenance and escalation
- Handling unreliable or incomplete context in production systems

Study focus:

- Designing systems that keep relevant memory without overloading context
- Understanding trade-offs between prompt context, retrieval, and tool-based sources of truth
- Building agent workflows that remain robust under incomplete or changing information

## What the exam is testing

This is not a memorization exam. The exam emphasizes architectural judgment in realistic scenarios.

You should be comfortable with:

- Choosing between prompt-based and tool-based approaches
- Assessing if a workflow is safe, deterministic, and maintainable
- Diagnosing architecture failures in agents and tool chains
- Designing robust agentic systems for business use cases

## Recommended study approach

### Phase 1: Foundation

- Review Claude Code workflows and repository conventions
- Study sample agent patterns for orchestration and tool calling
- Learn the difference between static prompt design and runtime orchestration

### Phase 2: Architecture patterns

- Practice designing multi-agent and tool-assisted systems
- Understand failure modes: tool errors, missing context, invalid outputs, and looping behavior
- Evaluate where human oversight and escalation should be built in

### Phase 3: Scenario practice

- Work through realistic exam-style situations
- Look for the most robust, production-friendly architecture decision
- Prefer solutions that are explainable, observable, and maintainable

## Practical prep checklist

- Understand the agent loop: request -> tool selection -> execution -> result -> iteration
- Learn how context is assembled and trimmed in real workflows
- Know what good MCP tool design looks like
- Be able to justify why a solution should use tools, retrieval, or tight validation logic
- Practice evaluating reliability and failure handling under production constraints

## Useful learning resources

- Anthropic partner/certification information: https://www.anthropic.com/partner
- Community study guide and practice questions: https://dnacenta.github.io/claude-certified-architect/guide_en.pdf
- Additional scenario-based study repo: https://github.com/scholarly360/claude-certified-architect-foundations
- Related reference material on Claude Code, MCP, and agent workflows from Anthropic docs

## Notes for this repository

This repo should be treated as a personal study notebook and index for the certification preparation journey. Add notes, architecture diagrams, prompts, checklists, and references here as the study process evolves.

## Suggested next steps

1. Review the official exam guide PDF and extract any updated details.
2. Add a personal summary of each domain with examples and anti-patterns.
3. Capture a set of scenario-based notes and wrong-answer explanations.
4. Build a lightweight study plan with weekly milestones.
5. Practice explaining why a solution is correct in production terms, not just technically plausible.

This repository is intended to support the learning process, not to replace official Anthropic certification materials.
