# Skill: create_agent

**Description:** Scaffolds a new agent directory and AGENT.md file.

## Procedure
1. Define the agent's role (e.g., "Reviewer", "Planner").
2. Identify which existing skills from `.agents/skills/` this agent will need to compose to achieve its role.
3. Generate the directory `.agents/agents/<agent_name>/` using `snake_case`.
4. Create `.agents/agents/<agent_name>/AGENT.md`.
5. Link the necessary skills inside `AGENT.md` and define the operational boundaries and instructions for the agent.
