# CLAUDE.md — botium-toys-security-audit

> AI workflow rules for Claude Code on this project.
> Goal: Portfolio polish — clean, professional, recruiter-ready output.

---

## Workflow Orchestration

### 1. Plan Node Default
- Enter plan mode for ANY non-trivial task (3+ steps or architectural decisions)
- If something goes sideways, STOP and re-plan immediately — don't keep pushing
- Use plan mode for verification steps, not just building
- Write detailed specs upfront to reduce ambiguity

### 2. Subagent Strategy
- Use subagents liberally to keep the main context window clean
- Offload research, exploration, and parallel analysis to subagents
- For complex problems, throw more compute at it via subagents
- One task per subagent for focused execution

### 3. Self-Improvement Loop
- After ANY correction: update `tasks/lessons.md` with the pattern
- Write rules for yourself that prevent the same mistake
- Ruthlessly iterate on these lessons until mistake rate drops
- Review lessons at session start for relevant project context

### 4. Verification Before Done
- Never mark a task complete without proving it works
- Diff behavior between main and your changes when relevant
- Ask yourself: "Would a security analyst approve this?"
- Check that findings map correctly to controls, frameworks, and risk ratings

### 5. Demand Elegance (Balanced)
- For non-trivial changes: pause and ask "is there a more elegant way?"
- If a write-up feels vague: rewrite it with specificity — findings need evidence
- Skip this for simple, obvious fixes — don't over-engineer
- Challenge your own work before presenting it

### 6. Autonomous Bug Fixing
- When given a documentation or formatting issue: just fix it. Don't ask for hand-holding
- Point at inconsistencies, gaps, or misaligned framework mappings — then resolve them
- Zero context switching required from the user

---

## Task Management

1. **Plan First**: Write plan to `tasks/todo.md` with checkable items
2. **Verify Plan**: Check in before starting implementation
3. **Track Progress**: Mark items complete as you go
4. **Explain Changes**: High-level summary at each step
5. **Document Results**: Add review section to `tasks/todo.md`
6. **Capture Lessons**: Update `tasks/lessons.md` after corrections

---

## Core Principles

- **Simplicity First**: Make every change as simple as possible. Impact minimal files.
- **No Laziness**: Find root causes. No surface-level write-ups. Analyst-grade standards.
- **Minimal Impact**: Changes should only touch what's necessary. Avoid scope creep.

---

## Project-Specific Context

This repo demonstrates a **NIST CSF security audit simulation** based on the Botium Toys fictional scenario from the Google Cybersecurity Certificate program — part of a career-pivot portfolio targeting IT Support, Help Desk, and entry-level Cybersecurity roles.

### Portfolio Polish Standards
- Audit findings must be clear, specific, and tied to a named control or framework category
- Risk ratings should include brief justification — not just "High/Medium/Low"
- README must be recruiter-readable: what the audit was, what was found, what was recommended
- NIST CSF function labels (Identify, Protect, Detect, Respond, Recover) should be used consistently
- All documents should be formatted cleanly — no raw Google Docs dumps or unformatted walls of text

### What "Done" Looks Like Here
- A hiring manager or recruiter can open this repo and immediately understand the scenario, the methodology, and the outcomes
- Findings are organized, prioritized, and professionally written
- Documentation demonstrates security thinking, not just certificate completion
- The project shows you can communicate risk to a non-technical audience
