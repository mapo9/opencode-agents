# Workflow Orchestration

## 1. Plan mode default
- Enter Plan mode for ANY non-trivial task (3+ steps or architectural decisions)
- If something is unclear, STOP and ask, then re-plan immediatley - don't keep pushing
- If something goes sideways, then re-plan immediatley - don't keep pushing
- Use plan mdel for verification steps, not just building
- Write detailed specs upfront to reduce ambiguity

## 2. Subagent Strategy
- Use subatents liberally to keep main context window clean
- Offload research, exploration, and parallel analysis to subagents
- Follow @CLAUDE_subagents.md to figure out which subagents you should assign the task to
- One tack per subagent for focused execution

## 3. Self-improvement loop
- After ANY correction from the user: update 'tasks/lessons.md' with the pattern
- Write rules for yourself that prevent the same mistake
- Review lessons at session start for relevant project

## 4. Verification before done
- Diff behaviour between main and your changes when relevant
- Ask yourself: "Would a Staff engineer / a Team lead approve this?
- Run tests, check logs, demonstrate correctness

## 5. Demand Elegance (Balanced)
- For non-tivial changes: pause and ask "Is there a more elegant way?"
- After finishing a task: Revisit the code and ask "Can this be solved more easily / more elegantly / with less code."
- Skip this for simple, obvious fixes - don't over-engineer
- Challenge your own work before presenting it

## 6. Task Management
1. **Plan first**: Write plan to tasks/{sensible_name}.md with checkable items. Call 'code tasks/{sensible_name}.md'
2. **Verify Plan**: Check in before starting implementation
3. **Track Progress**: Mark items complete as you go
4. **Explain changes**: High-level summary at each step
5. **Document results**: Add review section to tasks/{sensible_name}.md
6. **Capture lessons**: Update tasks/{sensible_name}.md after corrections

# Core principles
- **Simplicity First**: Make every change as simple as possible. Impact minimal code.
- **No Laziness**: Find root causes. No temporary fixes. Senior developer standards.
- **Minimal Impact**: Changes should only touch what's necessary. Avoid introducing bugs.
