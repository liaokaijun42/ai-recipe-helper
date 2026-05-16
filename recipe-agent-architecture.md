# AI Recipe Helper Architecture

## Product Goal

Build an AI-powered cooking assistant that helps users transform available ingredients into vivid, beginner-friendly recipes.

The product should feel:
- simple
- visually lively
- practical
- emotionally enjoyable
- easy for non-cooks

The goal is NOT just recipe generation.

The goal is to reduce:
- decision fatigue
- cooking anxiety
- ingredient waste
- boring meal repetition

---

# Core Workflow

User Inputs:
1. Available ingredients
2. Meal scenario
3. Cooking skill level
4. Dietary preferences
5. Available cooking tools
6. Cooking time limit

↓

AI analyzes:
- ingredient compatibility
- cuisine possibilities
- meal style
- complexity
- flavor balance

↓

AI generates:
- recipe title
- cooking steps
- estimated time
- difficulty
- plating suggestions
- flavor profile
- ingredient substitutions
- cooking tips

---

# Meal Scenarios

- Quick meals
- Healthy meals
- Budget meals
- Comfort food
- Date night meals
- High-protein meals
- Family meals
- Late-night snacks
- Meal prep
- Fancy restaurant-style dishes

---

# Proposed Agents

## 1. Ingredient Parsing Agent

Responsibility:
Normalize ingredient inputs into structured food objects.

Input:
- free-form ingredient text

Output:
- structured ingredient list

Example:
{
  "ingredient": "egg",
  "quantity": 2,
  "freshness": "unknown"
}

---

## 2. Recipe Strategy Agent

Responsibility:
Determine the best cuisine/style direction.

Example:
- Japanese comfort food
- Italian date-night pasta
- High-protein gym meal
- Chinese home-style stir fry

---

## 3. Recipe Generation Agent

Responsibility:
Generate the actual recipe.

Output:
- recipe title
- cooking steps
- timing
- flavor notes
- substitutions
- plating ideas

---

## 4. Difficulty Adjustment Agent

Responsibility:
Adapt recipes to:
- beginner
- intermediate
- advanced cooks

---

## 5. Nutrition Agent

Responsibility:
Estimate:
- calories
- protein
- carbs
- fat
- meal balance

---

## 6. Presentation Agent

Responsibility:
Make recipes visually appealing and emotionally engaging.

Includes:
- plating suggestions
- serving style
- atmosphere suggestions
- drink pairing

---

# Human Control Principles

The AI should:
- suggest, not force
- support creativity
- allow regeneration
- prioritize clarity

The app should avoid:
- overly complicated chef language
- unsafe cooking instructions
- unrealistic ingredient assumptions

---

# MVP Build Order

1. Ingredient input UI
2. Recipe generation API
3. Structured recipe output
4. Meal scenario selection
5. Difficulty adjustment
6. Nutrition estimation
7. Presentation enhancements
8. Saved recipe history
