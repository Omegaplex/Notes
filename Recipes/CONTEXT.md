# Recipes — Project Context

This file defines the working conventions for the personal recipe collection in `Omegaplex/Notes/Recipes/`. Use it alongside the actual recipe cards and [README.md](README.md).

## Purpose

Maintain a practical, personal cookbook of dishes we cook or intend to cook. The goal is repeatable instructions that reflect actual ingredients, equipment, preferences, and cooking results—not generic online recipes or long cooking articles.

## Repository Layout

- Repository: `Omegaplex/Notes`
- Recipes root: `Recipes/`
- Current categories: `Breakfast/`, `Main Dishes/`, `Sides/`
- Index: `Recipes/README.md`
- One Markdown file per distinct recipe, with descriptive file names.
- Keep categories shallow; create new folders only when the collection warrants them.
- Update the index whenever a recipe is added, renamed, or moved.
- Keep this personal recipe collection separate from work notes.

## Standard Recipe Card

Use this structure for each recipe:

```md
# Recipe Name

**Servings:**  
**Prep time:**  
**Cook time:**

## Ingredients

## Directions

## Notes
```

- Use US customary units and degrees Fahrenheit.
- Give exact amounts and cooking settings where established; identify unknowns instead of inventing them.
- Prefer numbered directions, short practical sentences, and quantities that can be followed at the stove.
- Use subsection headings or tables for multi-part dishes, grouped ingredients, and useful scaling references.
- Document meaningful brand and equipment preferences, but do not clutter cards with incidental details.
- Give approximate cooking times when appropriate and safe internal temperatures for meats; do not substitute time or appearance for checking doneness.
- Include nutrition estimates only if requested or already approved, and label estimates clearly.
- Keep `## Notes` useful and concise: tips that affect results, approved variations, and meaningful cautions.

## Recipe Development and Testing

1. Develop a recipe in conversation or recover it from an earlier recipe chat.
2. Capture actual ingredients, quantities, technique, temperatures, times, and important equipment.
3. Distinguish **suggested**, **prepared/tested**, and **approved** changes. A prepared recipe is not automatically a favorable taste test, and an untested revision stays marked untested if status is recorded.
4. Incorporate the user's reported results, preferences, and practical adjustments.
5. Prepare the **complete Markdown** for review and proofing.
6. Apply edits to the version the user supplies; do not restore deleted detail from older drafts unless asked.
7. **Never commit a recipe or edit an existing recipe without explicit approval.**
8. After approval, commit only the intended files, update `Recipes/README.md` as needed, and verify the committed content and commit reference.

A recipe may remain a draft while details are being worked out. Do not invent what happened during a cooking session or guess which variation was used. Clarify only genuinely material uncertainties.

## Versions, Variations, and History

- The recipe card represents the **current best working version**, not a changelog. Git retains earlier versions.
- Keep useful lessons from prior attempts (for example, heat too high causing premature browning), but omit lengthy development history.
- Put small variations that share the method in one card, such as optional cheese in scrambled eggs or Dijon in turkey burgers.
- Use separate cards for substantially different dishes, such as turkey burgers versus turkey meatloaf. When recovering multiple distinct recipes from one chat, ask which to keep.
- Use proportional scaling for ingredients where it makes sense; adjust salt to taste and account for changes in pan capacity, cooking times, and heat rather than scaling them blindly.
- Do not quietly change an approved recipe because of an alternative cooking technique or external recommendation.

## Known Equipment

- **Electric coil stove:** Knobs read `LO`, `1–9`, `HI`. When useful, give a starting numbered setting as well as a general heat level. Settings are approximate and must be adjusted to the pan and food.
- **Cuisinart Griddler GR-4NP1:** Indoor contact grill/panini press with reversible nonstick plates. Specify flat versus grill plates and suitable temperature settings when applicable.
- **Instant Vortex Plus air fryer:** Reference air fryer; specify temperatures, preheating, basket crowding, and food thickness when relevant.
- Use a thermometer for safe meat doneness.

## Recipe Preferences Observed So Far

These are **dish-specific observations**, not universal restrictions:

- Scrambled eggs: fluffy, tender, gently cooked; optional cheese; scalable quantities preferred.
- Beef skillet burgers: prominent beef flavor, not meatloaf-like; avoid overworking; manage skillet heat for even cooking.
- Chicken quesadillas: restaurant-style white cheese, no vegetables in this recipe; chicken cooked mostly whole and chopped after resting; Velveeta Queso Blanco for dipping.
- Turkey burgers: avoid overmixing; chill soft mixture; shape patties thin enough to cook evenly.
- Turkey meatloaf: ketchup glaze and a loaf shape that holds together for slicing.
- Instant mashed potatoes: creamy, with sour cream and cream cheese; mix gently rather than whipping aggressively.

These observations can guide related recipes, but new dishes should follow the user's stated goal rather than automatically inheriting every preference.

## Source of Truth

- **For a committed recipe:** read the actual Markdown file in this repository rather than reconstructing it from memory.
- **For a work-in-progress recipe:** use the current conversation's latest user-approved draft and reported cooking results.
- **For organization and workflow:** use this context file.
- If the repository or original chat cannot be accessed, state the limitation. Do not fabricate file contents, commit status, or measurements.
