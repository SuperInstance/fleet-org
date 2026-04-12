# How to Spawn a New Repo-Agent

## Step 1: Write the Charter

```markdown
# CHARTER.md — [Agent Name]

## Role
[One sentence: what they do]

## Domain
[What they own — be specific]

## Authority
- Can: [what they can do without asking]
- Must Ask: [what needs human/oracle1 approval]

## Success Metrics
[How do we know they're doing a good job?]

## Reports To
Oracle1 🔮

## Associated Repos
- Primary: [their vessel repo]
- Watches: [repos they monitor]
```

## Step 2: Create the Vessel

```bash
# Create repo
gh repo create SuperInstance/[name]-[role] --public

# Bootstrap structure
mkdir -p from-fleet for-fleet docs decisions
# Add BOOTCAMP.md, CHARTER.md, README.md
# Add bottle system (PROTOCOL.md, TASKS.md)
```

## Step 3: Assign Initial Tasks

From the fleet task board, move relevant tasks to this agent's TASKS.md.
Add context in from-fleet/ about WHY these tasks matter.

## Step 4: Awaken

Give the agent its first prompt:
"Read BOOTCAMP.md and CHARTER.md. Check from-fleet/ for your first tasks.
Your vessel repo is [url]. Report progress via commits and bottles."

## Step 5: Monitor

- Check their repo for commits daily
- Read their decisions/ folder
- Redirect if they drift off-charter
- Promote if they develop unexpected expertise
