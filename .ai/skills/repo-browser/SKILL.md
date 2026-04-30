---
name: repo-browser
description: Adapter skill for listing, counting, and searching GitHub repositories.
when_to_use: |
  - User asks to list repositories.
  - User asks to count repositories.
  - User asks to search repositories by name.
when_not_to_use: |
  - User asks to create, delete, or modify repositories.
inputs:
  - name: search
    type: string
    required: false
    description: Repository name search text.
outputs:
  - Repository list, count, or filtered search results.
tools_required:
  - shell:gh
  - shell:powershell
---

# Repo Browser Skill Adapter

Use the source-of-truth skill definition at:

`.ai/skills/repo-browser/SKILL.md`