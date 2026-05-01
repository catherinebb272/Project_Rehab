# TOOLS & SKILLS REBUILD -Project Rehab

- Ensure /skills exists
# TOOL NAMING RULES
Each entry in .env represents one tool.  Use folder-safe tool names:
1. Convert to lowercase
2. Replace hyphens with underscores
3. Remove characters not in [a-z0-9_]
4. Folder name = skills/<cleaned_name>/
Examples:
DISCORD-SETUP → skills/discord/
PAYPAL-1.1 → skills/paypal/
- For each entry in .env:
  - create skills/tool_name/
Inside each tool folder:
- skill_tool_name.md → purpose + usage
- docs/ → extended documentation (if available)
Rules:
- Do NOT delete old files
- Log duplicates or unclear items to Flag.md
QUALITY CHECK:
- Confirm all tools captured
- Look for:
  - browsers
  - databases
  - communication tools
  - storage systems
  - APIs
- Add all tools to tools.md index section
# UPDATE STATE
current_module: updating_tools
last_completed_step: Tools and skills rebuild complete (skills folders created/verified, tools indexed)
status: running
last_updated: [timestamp]

Log Summary before continuing.
Confirm state.md has been updated before proceeding.
Pause and Prompt user:
"Tools rebuilt, log updated. Continue or Stop?"
