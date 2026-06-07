# Day 7 — Building a Personalized Claude AI Usage Strategy Generator

## What I Built Today

Today I created an **interactive Claude AI Usage Strategy Generator** — a React-based artifact that analyzes a user's profile (role, activities, usage frequency, and output needs) and generates a fully personalized Claude model + effort level recommendation system.

The app outputs a clean, visual strategy dashboard with three tabs:
- **Strategy** — Primary model recommendation, when to use Haiku / Sonnet / Opus, and effort level breakdown
- **Workflow** — A full task-to-model-to-effort mapping table + an ideal daily routine
- **Mistakes** — Common pitfalls to avoid and a final single-model recommendation

---

## Tech Stack

- **React** (functional components + hooks)
- **Claude API** via Anthropic (`claude-sonnet-4-20250514`)
- **Inline CSS** for dark-theme, production-grade UI
- **Interactive prompt flow** using Claude's `ask_user_input_v0` tool for structured user profiling

---

## My Profile & Output

**Inputs collected:**
| Question | My Answer |
|----------|-----------|
| Current Situation | Student |
| Primary Activities | Coding, Research & Learning, Marketing & Business Planning |
| Usage Frequency | Daily |
| Output Type Needed | Deep Research / Business Strategy |

**Final Recommendation Generated:**
> **Claude Sonnet + Standard Effort** as the primary daily driver, with Opus + High effort reserved for deep research, business plans, and high-stakes outputs.

---

## Key Learnings

### Claude Model Tiers (What I Actually Understood Today)

| Model | Best For | When to Avoid |
|-------|----------|---------------|
| **Haiku** | Quick lookups, summaries, simple rewrites | Complex reasoning, deep research |
| **Sonnet** | Daily coding, research, content, study help | Ultra-complex multi-step architecture |
| **Opus** | Business strategy, literature reviews, critical essays | Routine tasks (overkill + burns limits) |

### Effort Levels Decoded

- **Low** → Simple tasks, fast answers
- **Standard** → 70–80% of all daily work
- **High** → Complex problems that need structured multi-step reasoning
- **Max** → Only for truly high-stakes outputs (final essays, major decisions)

---

## Challenges I Faced During Generation

### 1. Designing the Prompt Flow
Getting the 4-question profiling system to feel natural was tricky. I had to think carefully about which questions would give enough signal to generate a meaningful, personalized strategy — without overwhelming the user.

### 2. Mapping Activities to Models Correctly
The user profile (Student + Coding + Research + Business Planning + Daily) touched all three Claude tiers. Deciding when Sonnet was "enough" vs. when Opus was truly needed required thinking through real use cases, not just general rules.

### 3. UI Without a Design System
Building a dark-themed, multi-tab React UI entirely with inline CSS (no Tailwind compiler, no external component library) meant manually handling every spacing, color, border, and animation decision. Getting the tab switching, color-coded model cards, and animated effort bars right took careful iteration.

### 4. Making It Beginner-Friendly Without Dumbing It Down
The goal was "clean, visual, beginner-friendly" — but the content (model tiers, effort levels, workflow optimization) is inherently technical. Balancing depth with accessibility in the copy and layout was a real design challenge.

### 5. Effort Level Naming Confusion
During generation, I realized Claude's effort settings aren't universally labeled the same way across all interfaces. I had to make judgment calls about how to present Low / Standard / High / Max in a way that felt intuitive and actionable for a student user.

---

## What I'd Improve Next

- [ ] Add a "Save my strategy" feature using persistent storage
- [ ] Let users re-run the quiz and compare strategies
- [ ] Add real-time Claude API integration so the strategy itself is generated dynamically by Claude based on the profile
- [ ] Include cost/usage estimates per model tier

---

## Reflection

This project pushed me to think not just about *how* to use Claude, but *why* different tasks deserve different tools. The biggest mindset shift: **matching the right model to the right task is itself a skill** — and most people (including me before today) default to one model for everything and leave a lot of value on the table.

The hardest part wasn't the code — it was the product thinking behind designing a system that gives genuinely useful, personalized advice rather than generic recommendations.

---

*Day 7 of my AI/Claude learning journey 🚀*
