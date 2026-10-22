# Skill: create_skill

**Description:** Scaffolds a new skill directory and SKILL.md file adhering strictly to agent conventions.

## Procedure
1. Ask the user for the narrow purpose of the skill.
2. Check if the logic branches too much (if yes, suggest splitting into multiple skills).
3. Generate the directory `.agents/skills/<skill_name>/` using `snake_case`.
4. Create `.agents/skills/<skill_name>/SKILL.md` populated with brief, dense instructions on how to execute the skill.
5. Scaffold a `reference/` directory alongside `SKILL.md` for any long code examples or schemas.
