# TECHNICAL LOG & INTRODUCTION TO AGENT SKILLS

## AGENT SKILLS ON CLAUDE
**CCNP Miguelangel Luna**

---

## CONTENT:

| Case | Title | Description |
| :--- | :--- | :--- |
| **01** | [Claude & n8n AI Agents](./case-01-Google-Auth/) | Agentes Claude |

[Antrophic](https://anthropic.skilljar.com/introduction-to-agent-skills/434527)

## 1. Introduction and Theoretical Framework:

**What is a Skill?**

A Skill is a local directory containing a file named **`SKILL.md`**. This file instructs **Claude Code** on how to consistently execute a task across your projects.

**Structure of the SKILL.md File:**

The file consists of **two main sections separated by YAML metadata** (frontmatter):

- **Metadata (Frontmatter):** Defines the `name` and `description`. Claude uses the description to semantically evaluate when to trigger the skill.
- **Instructions:** Instructions written in Markdown that execute the desired workflow when the skill is activated.



## 2. Topology and BGP Neighbor Establishment

The topology consists of four routers across different Autonomous Systems .

![BGP WEIGTH](images/01Topologia.jpg)


## 3. Creating a Skill:

3.1) First, create a directory for your skill inside the skills folder. **The directory name should match your skill name**:

**3.1)** Create a directory:

```text
nano ~/.claude/skills/pr-description/SKILL.md
```

**3.2)** Then create a **`SKILL.md`** file inside that directory. The file has two parts separated by frontmatter dashes:

```text
nano ~/.claude/skills/pr-description/SKILL.md
```
**3.3)**

---
name: pr-description
description: Generates professional and structured Pull Request (PR) descriptions based on git diffs or commit summaries.
---

# PR Description Generator Guidelines

When generating a Pull Request description, always follow this standard structure:

```text
1. **Title:** Clear, imperative summary (e.g., *Fix authentication token expiration handling*).
2. **Type of Change:** Select one (Feature, Bug Fix, Refactoring, Documentation, Performance).
3. **Description:** A concise explanation of *what* was changed and *why*.
4. **Testing Done:** How the changes were tested locally or in staging.
5. **Checklist:**
   - [ ] Tests added/updated
   - [ ] Documentation updated
   - [ ] Code follows project style guidelines
```

### 4. BGP Configuration:


