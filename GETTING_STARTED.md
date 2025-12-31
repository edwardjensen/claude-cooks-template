# Getting Started

This guide will help you set up your personalized culinary knowledge base for use with Claude.

## Prerequisites

- A GitHub account (to fork/clone this repository)
- [Claude Code](https://claude.ai/code) CLI or access to [Claude.ai](https://claude.ai)
- A text editor for filling in your information

## Quick Setup

### 1. Fork or Clone This Repository

```bash
# Option A: Fork on GitHub, then clone your fork
git clone https://github.com/YOUR_USERNAME/claude-cooks.git

# Option B: Clone directly and set your own remote
git clone https://github.com/ORIGINAL/claude-cooks-template.git claude-cooks
cd claude-cooks
git remote set-url origin YOUR_NEW_REPO_URL
```

### 2. Start with Your Profile

Open `core/profile.md` and fill in:

- **Household overview** — Are you cooking for one, a couple, or a family?
- Your location (affects seasonal ingredient availability)
- Your skill level (helps Claude calibrate complexity)
- **Dietary requirements:**
  - Allergies & medical (safety-critical)
  - Religious/cultural (halal, kosher, etc.)
  - Lifestyle diets (vegetarian, keto, etc.)
  - Preferences (dislikes, can be overridden)

This is the most important file—it ensures Claude never suggests something unsafe or inappropriate for your household.

### 3. Document Your Equipment

Open `core/equipment.md` and list:
- Your stovetop and oven setup
- Any special equipment (stand mixer, sous vide, instant pot, etc.)
- General inventory overview

This helps Claude suggest recipes that match your actual kitchen capabilities.

### 4. Add Your Local Stores

Open `shopping/sources.md` and fill in:
- Your preferred warehouse/bulk store
- Regular grocery stores
- Specialty grocers
- Farmers markets and schedules
- Any ethnic/cultural markets you frequent

This enables Claude to organize shopping lists by store.

### 5. Populate Staples (Ongoing)

The staples files (`core/pantry-staples.md`, `core/fridge-staples.md`, `core/freezer-staples.md`) can be filled in over time. Start with what you know you always have on hand.

## File Priority Guide

| Priority | Files | Why |
|----------|-------|-----|
| **Do First** | `core/profile.md` | Safety (allergies) and basic context |
| **Do Second** | `core/equipment.md`, `shopping/sources.md` | Practical recipe matching |
| **Do Third** | Staples files in `core/` | Enables "what can I make with what I have" queries |
| **Do Later** | `contexts/` files | Situational fine-tuning |
| **Do Later** | `shopping/errand-strategy.md` | Shopping optimization |
| **Review Only** | `output/` files | Adjust if you want different formatting/tone |

## How to Use

Once you've filled in your information, use Claude with this repository as context.

### With Claude Code CLI

```bash
cd your-claude-cooks-directory
claude
```

Claude Code will automatically read `CLAUDE.md` and have access to your files.

### With Claude.ai

Upload the relevant files or copy their contents into your conversation when asking culinary questions. If the files are in your GitHub account, you can connect the repository directly to Claude.ai for easier access.

### Example Prompts to Try

- "What can I make for dinner tonight with what's in my pantry and fridge?"
- "Plan a Sunday meal prep session for the week ahead"
- "I'm hosting 6 people for a casual dinner party—suggest a menu"
- "I want to learn a new technique this weekend. What should I try?"
- "Create a shopping list for [recipe], organized by my stores"

## Tips

- **Iterate over time.** You don't need to fill everything in at once. Start with the essentials and add detail as you cook.
- **Update as things change.** New equipment? Different store preferences? Keep your files current.
- **The `contexts/` files are optional.** They add nuance but aren't required for basic functionality.
- **Customize the output files.** If you prefer metric measurements or a different voice, edit `output/recipe-format.md` and `output/tone-and-style.md`.

## Need Help?

If you have questions about this template, open an issue on the repository.
