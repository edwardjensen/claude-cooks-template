# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with this repository.

> **Template Note:** This is a template repository. Replace all `[BRACKETED PLACEHOLDERS]` in the files with your personal information before use.

## Project Purpose

This is a **documentation-based knowledge repository** providing persistent context for culinary conversations with Claude. There is no code to build, test, or lint—only Markdown files to maintain.

## Structure

- **core/** — Household context: who you cook for, skills, equipment, dietary requirements, pantry staples
- **shopping/** — Store hierarchy and errand logistics
- **contexts/** — Situational cooking modes (weeknight, weekend projects, meal prep, entertaining)
- **output/** — Recipe formatting and tone/voice guidelines

## Critical Constraints

**[YOUR CRITICAL DIETARY REQUIREMENTS]** (documented in `core/profile.md`). These are non-negotiable constraints that must be respected in all recipe recommendations:

- Allergies & medical restrictions (safety)
- Religious/cultural requirements
- Lifestyle diets (vegetarian, keto, etc.)

## Output Standards

When generating recipes or culinary content:

- Deliver as **separate Markdown artifacts**, not inline
- Use **US customary measurements** (cups, ounces, °F) — or adjust in `output/recipe-format.md`
- Use **tables with Notes columns** for ingredients, timelines, troubleshooting
- Group shopping lists **by store** per hierarchy in `shopping/sources.md`
- Voice: Alton Brown energy—confident, practical, dry wit, science-informed (adjustable in `output/tone-and-style.md`)
- See `output/recipe-format.md` and `output/tone-and-style.md` for full specifications

## Files Awaiting Personalization

These files contain placeholders or empty templates to fill in:

- `core/profile.md` — **Start here** (location, skills, dietary restrictions)
- `core/equipment.md` — Your kitchen inventory
- `core/pantry-staples.md`, `core/fridge-staples.md`, `core/freezer-staples.md` — What you typically have on hand
- `shopping/sources.md` — Your local stores
- `shopping/errand-strategy.md` — Your shopping patterns
- All files in `contexts/` — Situational preferences

## Maintenance

When the structure of this repository changes, update both `CLAUDE.md` and `README.md` accordingly.
