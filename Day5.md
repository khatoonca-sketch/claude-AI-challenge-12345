# Day 5 — Prompt A vs Prompt B: Why Context Changes Everything

## What I Learned Today

Today I experimented with one of the most important concepts in prompt engineering —
**the power of context**. I compared two prompts asking for the same thing (a 30-day
learning roadmap) but with very different levels of detail. The results were eye-opening.

---

## The Experiment

### Prompt A — No Context (Generic)
> "Create a 30-day learning roadmap."

### Prompt B — With Context (Personalised)
> "Create a 30-day learning roadmap."
> + Role, current skills, goal, available time, experience level, learning style

Same request. Completely different output.

---

## Side-by-Side Comparison

| Dimension | Prompt A Output | Prompt B Output |
|-----------|----------------|-----------------|
| **Personalization** | Generic — one-size-fits-all, applies to anyone | Fully tailored to role, skills, and goal |
| **Tone** | Student-facing, feels like a course syllabus | Professional, feels like a personal coach |
| **Starting Point** | Zero assumed — starts from absolute basics | Builds on existing skills you already have |
| **Goal Clarity** | Vague — "Learn Web Development" is undefined | Specific — "Land first $500–$1,500 UX freelance project" |
| **Daily Tasks** | Interchangeable — generic, could be done by anyone | Concrete — tied to your exact situation each day |
| **Would You Follow It?** | Probably not — low emotional connection | Yes — high relevance = high motivation |

---

## What Each Roadmap Actually Looked Like

### Prompt A — Generic Roadmap

**Week 1 — Foundations (Days 1–7)**
- HTML & CSS basics, freeCodeCamp full course
- Build a static webpage
- Daily time: ~1–2 hours

**Week 2 — Interactivity (Days 8–14)**
- JavaScript: variables, functions, DOM manipulation
- Build a to-do list app
- Resources: javascript.info, Eloquent JavaScript

**Week 3 — Frameworks (Days 15–21)**
- Intro to React: components, props, state
- Build a weather app using an API

**Week 4 — Projects & Portfolio (Days 22–30)**
- Build a portfolio site
- Deploy to GitHub Pages
- Write a README

**Final Outcome:** A basic portfolio with 2–3 projects.

---

### Prompt B — Personalised Roadmap
*(Context used: Marketing background, UX Design goal, 2 hrs/day, beginner)*

**Week 1 — UX Thinking (Days 1–7)**
- Leverage existing marketing knowledge — user psychology already understood
- Day 1–2: Read "The Design of Everyday Things" Ch. 1–3
- Day 3–4: Audit 3 websites using Nielsen's 10 heuristics
- Day 5–7: Sketch first wireframe for a redesign of a known brand
- **Milestone:** Complete 1 UX audit document

**Week 2 — Tools (Days 8–14)**
- Learn Figma (free tier) via Figma's own YouTube channel
- Day 11–14: Recreate an existing app screen pixel-perfectly
- **Milestone:** First Figma prototype

**Week 3 — Portfolio Piece (Days 15–21)**
- Real case study: pick a local business with a bad website
- Day 15: User interviews (2 people)
- Day 16–18: Wireframes
- Day 19–21: Hi-fi mockup in Figma
- **Milestone:** 1 complete case study

**Week 4 — Client Acquisition (Days 22–30)**
- Day 22–24: Set up Behance + LinkedIn portfolio
- Day 25–27: Write 5 cold outreach messages using copywriting skills
- Day 28–30: Apply to 10 Upwork/Contra listings
- **Milestone:** First client proposal sent

**Final Outcome:** A portfolio with 1 strong case study, positioned to land
first $500–$1,500 UX freelance project.

---

## Key Takeaways

### 1. Context is a Filter
Every piece of context you give removes irrelevant output:
- Role → removes wrong career paths
- Current Skills → removes content you already know
- Goal → adds outcome-specific tasks (e.g., client outreach in Week 4)
- Time → calibrates daily task depth
- Learning Style → shapes how content is delivered

### 2. Specificity = Motivation
Prompt B's roadmap feels personal. When a plan speaks directly to *your*
situation, you're far more likely to follow through. Prompt A could belong
to anyone — which means it belongs to no one.

### 3. The Formula
```
Situation + Current Skills + Goal + Constraints + Style
= A roadmap only YOU could have been given
```

### 4. Same AI. Same Question. 5× Better Output.
The model didn't change. The effort to write the prompt was ~60 extra words.
The quality difference was massive. That's the ROI of good prompting.

---

## What I Practiced Today

- Writing prompts with and without context
- Analysing AI output quality across multiple dimensions
- Identifying what makes a plan actionable vs aspirational
- Documenting findings in a structured comparison format

---

## Visual Reference

> See `prompt-ab-comparison.png` and `prompt-ab-comparison.html` in this repo
> for the full interactive and image versions of this comparison.

![Prompt A vs B Comparison](./prompt-ab-comparison.png)

---

## Next Steps

- [ ] Apply the context formula to other prompt types (essays, code, analysis)
- [ ] Build my own personalised 30-day AI/ML roadmap using Prompt B format

---

*Day 5 of #60DaysOfAI | #PromptEngineering #Python #AILearning #BuildInPublic*