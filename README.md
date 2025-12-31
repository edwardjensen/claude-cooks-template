# Claude Cooks Template

![Overhead food photography of a healthy grain bowl with grilled salmon, green beans, couscous, cherry tomatoes, and pine nuts on a pink plate atop a wooden cutting board, with a small bowl of tomatoes to the left and pesto sauce to the right. Text reads \"CLAUDE COOKS!\"
](claudecooks.jpeg)

A template for creating a personalized culinary knowledge base for AI-assisted cooking with Claude.

## What Is This?

This repository provides a structured framework for giving Claude persistent context about your cooking preferences, kitchen setup, dietary restrictions, and local shopping options. Instead of re-explaining your situation in every conversation, you fill in these files once and Claude has the context it needs.

**[Get Started →](GETTING_STARTED.md)**

## How to Use This Template

1. **Fork or clone** this repository
2. **Fill in your information** starting with `core/profile.md`
3. **Use with Claude** via Claude Code CLI or by sharing files in Claude.ai

See [GETTING_STARTED.md](GETTING_STARTED.md) for detailed setup instructions.

## Structure

```text
claude-cooks/
├── core/                    # Your household context
│   ├── profile.md           # Who you cook for, dietary requirements, skills
│   ├── equipment.md         # Kitchen inventory and capabilities
│   ├── pantry-staples.md    # Shelf-stable items typically on hand
│   ├── fridge-staples.md    # Refrigerated items typically on hand
│   └── freezer-staples.md   # Frozen items typically on hand
├── shopping/                # Sourcing and logistics
│   ├── sources.md           # Store hierarchy and specialty callouts
│   └── errand-strategy.md   # Batch shopping and route optimization
├── contexts/                # Situational cooking modes
│   ├── weeknight-solo.md    # Quick meals after work
│   ├── weekend-projects.md  # Ambitious cooking sessions
│   ├── meal-prep.md         # Batch cooking for the week
│   └── entertaining.md      # Hosting guests
└── output/                  # Response formatting preferences
    ├── recipe-format.md     # Recipe structure and shopping lists
    └── tone-and-style.md    # Voice and creative parameters
```

## Example Use Cases

Once you've personalized your files, try conversations like:

- **Quick weeknight dinner**: Share `core/profile.md` + `contexts/weeknight-solo.md`
- **Planning a dinner party**: Share `core/profile.md` + `shopping/sources.md` + `contexts/entertaining.md`
- **Weekend batch cooking**: Share `core/profile.md` + `shopping/errand-strategy.md` + `contexts/meal-prep.md`

## Important: Dietary Requirements

Document all dietary requirements in `core/profile.md`. The file includes sections for:

- **Allergies & medical** — Safety-critical, never violated
- **Religious/cultural** — Halal, kosher, etc.
- **Lifestyle diets** — Vegetarian, keto, etc.
- **Preferences** — Dislikes that can be overridden if needed

For households with multiple people, list everyone's critical restrictions — they all apply.

## Customization

- **Output format**: Edit `output/recipe-format.md` to change how recipes are structured
- **Voice/tone**: Edit `output/tone-and-style.md` to adjust Claude's personality
- **Add new contexts**: Create additional files in `contexts/` for situations not covered

## License

[MIT](LICENSE)

## Photo credit

Photo by Ella Olsson on [Unsplash](https://unsplash.com/photos/vegetable-salad-KPDbRyFOTnE?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
