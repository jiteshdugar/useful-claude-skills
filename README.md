# 11 Most Useful Claude Skills

What each skill does, how it helps, and a ready-to-use prompt for each.

---

## 1. Caveman Mode

### What it's used for
Processing massive volumes of information—dozens of research papers, PDFs, articles, or decks—using minimal tokens.

### How it helps
- Prevents you from hitting Claude's conversation token limit prematurely.
- Maximizes daily usage (effectively doubling your capacity on the same plan).
- Delivers highly concise summaries without sacrificing data quality.

### Prompt
> Using the caveman mode, analyze these **[number]** research papers/documents on **[topic]**. Summarize the top tactics working right now ranked by impact, and cite the original source for each while keeping token usage to a minimum.

---

## 2. Find Skill

### What it's used for
Searching and matching the right skill from Claude's library for any task described in plain language.

### How it helps
- Eliminates the need to memorize or manually search through hundreds of skills.
- Acts as an automated dispatcher for specialized tools.

### Prompt
> Write a LinkedIn post about **[recent news/topic]**. Find me the right skill to write this in a high-performing post format.

---

## 3. Brand Guidelines

### What it's used for
Storing a brand's entire visual and voice identity (hex codes, font pairings, tone rules, and words to avoid) as a permanent skill.

### How it helps
- Eliminates repeatedly entering brand context.
- Keeps all content and visuals aligned with brand guidelines across clients and projects.

### Prompt
> Here is our brand profile: **[voice, colors, typography, audience, disallowed words]**. Lock this in as a permanent Brand Guidelines skill, complete with hex codes, font pairings, seven sample sentences, and examples of what **not** to sound like.

---

## 4. Fact Checker

### What it's used for
Verifying factual statements, claims, headlines, and statistics before publishing.

### How it helps
- Prevents misinformation.
- Checks every claim against authoritative sources.
- Provides confidence scores and citations.

### Prompt
> Fact-check this post/article: **[paste text]**. Extract every factual statement, verify each one against authoritative sources, assign a confidence score, and provide direct links to the verified sources.

---

## 5. SEO Skill

### What it's used for
Conducting technical SEO audits, competitor benchmarking, and AI search readiness assessments.

### How it helps
- Replaces expensive SEO audits.
- Identifies technical issues.
- Prioritizes fixes based on impact.

### Prompt
> Run a full technical SEO audit on **[your website]** and compare it against **[competitor 1]** and **[competitor 2]**. Show pillar scores, broken technical elements, AI search readiness, and a prioritized checklist of fixes.

---

## 6. Office Hours (Garry Tan / YC)

### What it's used for
Simulating a Y Combinator office hours session to stress-test business ideas.

### How it helps
- Provides brutally honest feedback.
- Challenges assumptions.
- Identifies weaknesses before investing time or money.

### Prompt
> Act as a Y Combinator partner during Office Hours. Grill my business (**[product description]**) with forcing questions around demand, market wedge, defensibility, retention, and growth strategy.

---

## 7. Skill Creator

### What it's used for
Building and packaging custom Claude skills for repeatable workflows.

### How it helps
- Lets non-technical users create reusable AI skills.
- Interviews you to understand the workflow before generating the skill.

### Prompt
> I want to create a custom skill for **[workflow]**. Interview me step by step about what success looks like, what red flags to watch for, then draft and package the skill.

---

## 8. The Humanizer

### What it's used for
Rewriting AI-generated content to sound natural and human.

### How it helps
- Removes AI clichés and predictable phrasing.
- Improves readability and response rates.
- Produces more authentic writing.

### Prompt
> Humanize the following draft: **[paste copy]**. Remove predictable AI writing patterns, generic buzzwords, and structural clichés while making the writing natural and concrete.

---

## 9. Deep Research

### What it's used for
Running multi-agent market research across competitors, pricing, funding, market size, and opportunities.

### How it helps
- Compresses weeks of consulting work into minutes.
- Cross-verifies information.
- Produces actionable GTM recommendations.

### Prompt
> Conduct a deep research report on building a **[product idea]** for **[target audience]** priced at **[price tier]**. Analyze market size, competitors, pricing, underserved opportunities, and recommend a go-to-market strategy.

---

# Claude Code Specific Skills

Installed as `SKILL.md` files inside a project's `.claude/skills/` folder and used within Claude Code to operate on real codebases.

---

## 1. Taste Skill

### What it's used for
Giving Claude Code a design and quality "eye" for frontend development.

### How it helps
- Avoids generic AI-generated UI.
- Infers design direction from audience and context.
- Maps designs to established systems (Fluent, Carbon, GOV.UK, shadcn, etc.).
- Can audit existing frontend implementations.

### Prompt
> In Claude Code, install the Taste skill (`npx skills add <repo> --skill taste-skill --agent claude-code`) and redesign the `/dashboard` route. Infer the design direction from the brief, avoid generic AI defaults, and give me a one-line design assessment before changing the code.

---

## 2. Emil Kowalski Skill

### What it's used for
Implementing polished animations and motion design directly in a codebase.

### How it helps
- Applies professional animation principles.
- Improves easing, timing, and GPU-accelerated transitions.
- Supports accessibility with `prefers-reduced-motion`.
- Enhances modals, toasts, hover effects, gestures, and transitions.

### Prompt
> In Claude Code, use the Emil Kowalski animations skill to audit and improve the animations in `src/components/Modal.tsx` and `src/components/Toast.tsx`. Improve easing, timing, and property choices, respect reduced-motion settings, and provide a before/after summary of the improvements.
