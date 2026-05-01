# CONTROLLER - PROJECT REHAB 
# STARTUP LOGIC
1. Check for state.md
   - If not found → create using initial template
2. Read state.md:
   - If status = complete → ask user if they want to restart
   - If paused or running → resume from current_module
3. Load idempotency_rules.md and follow all rules
Ensure that each module updates state.md with the next module in the execution flow.
Tools Module
Goal: Reorganize tools, skills, and files to eliminate disorganization-based forgetfulness.
Modules:
1. Prep → prep.md
2. Teach Behavior → teach_behavior.md
3. API Consolidation → api_consolidation.md
4. Tools Rebuild → tools_rebuild.md
5. Updating Tools Routine → updating_tools.md
Execution Flow:
- Run prep.md
- Ask user to continue or stop
- If continue → run teach_behavior.md
- Ask user to continue or stop
- If continue → run api_consolidation.md
- Ask user to continue or stop
- If continue → run tools_rebuild.md
- Ask user to continue or stop
- If continue → run updating_tools.md
At any STOP → run stop_routine.md
At completion → run stop_routine.md

# ON STOP
Update state.md:
status: paused
last_completed_step: [describe where stopped]
last_updated: [timestamp]

