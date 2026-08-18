# AGENTS.md — ThaiSub Brain Vault

## Overview
This vault contains Thai-translated video course subtitles and YouTube translations.
Each note has YAML frontmatter with course, lesson, and media metadata.

## Structure
- `Courses/` — Course lessons organized by course name
  - `AI-Automations-and-Agent-Templates/` — 141 lessons (6 translated)
  - `NoeAI/` — 126 lessons (12 translated)  
  - `Google-Ads-PPC/` — 380 lessons (0 translated)
- `YouTube/` — YouTube video translations
- `ThaiSub Brain.md` — Dashboard / home note

## Note Format
Each lesson note contains:
- YAML frontmatter: course, lesson, has_voiceover, has_subtitles, status, tags
- `## 📝 คำแปล` — Full Thai translation
- `## ⏱️ ซับไตเติ้ล (Timestamped)` — Timestamped subtitle segments
- Embedded audio: `![[filename.mp3]]` (Thai voiceover)

## AI Agent Guidelines
- When creating notes, follow the existing frontmatter format
- Tags should include `thai-sub` and the course folder name
- Audio files go in `attachments/` subfolder alongside the note
- Translations should be natural Thai, not literal
- Timestamps use format `HH:MM:SS`
