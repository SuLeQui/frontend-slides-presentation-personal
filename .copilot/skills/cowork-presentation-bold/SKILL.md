---
name: cowork-presentation-bold
description: Create distinctive, executive-grade HTML slide decks with strong visual direction and clear comparison storytelling. Use when the user asks for presentations that should avoid generic layouts and look intentionally designed.
---

# Cowork Presentation Bold

Create self-contained, animation-aware HTML presentations for business storytelling with strong visual character.

## Core Principles

1. Single file output. Use one HTML file with inline CSS and JS.
2. Strong visual identity. Pick one clear art direction and commit to it.
3. No generic defaults. Avoid interchangeable card-grid look and default font stacks.
4. Viewport discipline. Every slide must fit in 100vh with no internal scrolling.
5. Explain by contrast. When comparing products, design each comparison slide to be readable in under 10 seconds.

## Visual Direction Rules

1. Typography:
- Use expressive display font for headings and a readable sans for body.
- Never use Arial, Roboto, Inter, or system fallback as primary identity.

2. Color system:
- Define CSS variables in :root.
- Use one dominant color family plus one high-contrast accent.
- Include subtle atmospheric background layers (gradient, pattern, glow, or texture).

3. Composition:
- Alternate slide rhythms: hero, split-screen, matrix, quote, decision flow.
- Do not repeat the same card layout for more than two slides in a row.

4. Motion:
- Use one entrance choreography pattern and repeat consistently.
- Keep animation functional, not decorative noise.
- Include prefers-reduced-motion handling.

## Mandatory Layout Constraints

1. .slide must include:
- height: 100vh;
- height: 100dvh;
- overflow: hidden;

2. All text sizing and spacing must use clamp().

3. Responsive breakpoints required for:
- max-height: 700px
- max-height: 600px
- max-height: 500px

4. Maximum content density:
- Title slide: 1 title + 1 subtitle + optional CTA
- Standard slide: 1 heading + max 5 bullets or 3 cards
- Comparison matrix: max 4 products x max 5 rows
- Quote slide: quote + attribution only

If limits are exceeded, split into additional slides.

## Workflow

### Phase 1: Intake
Ask in one batch:
1. Audience: Executive / Technical / Mixed
2. Goal: Inform / Decide / Persuade
3. Length: 6-8 / 9-12 / 13+
4. Tone: Formal / Energetic / Visionary
5. Must-include points

### Phase 2: Narrative Structure
Build outline with this structure:
1. Context
2. Core concept
3. Comparison
4. Decision guidance
5. Rollout or next step

### Phase 3: Style Selection
Offer 3 style routes with one-line rationale each:
1. Editorial Contrast (clean, sharp, data-forward)
2. Signal and Steel (dark, high-contrast, decisive)
3. Soft Future (light, airy, strategic)

### Phase 4: Build
Generate full presentation HTML with:
1. Inline CSS and JS only
2. Keyboard navigation (arrows, space)
3. Dot navigation
4. Section comments in CSS and HTML
5. Source note slide when external references are used

### Phase 5: QA Checklist
Verify before delivery:
1. No slide overflow at 1280x720 and common laptop sizes
2. No crowded slide beyond density limits
3. Clear contrast ratio for heading and body text
4. Product comparisons remain neutral and factual
5. If preview features are mentioned, clearly label as preview

## Comparison Guidance for Copilot Topics

When presenting Copilot Cowork, Microsoft 365 Copilot, Microsoft Scout, and custom Copilot Studio agents:

1. Compare across the same dimensions:
- Primary purpose
- Best-fit scenarios
- Execution model
- Control and governance
- Typical effort to adopt

2. Use this decision framing:
- Single-step assistance -> Microsoft 365 Copilot
- Multi-step M365 execution -> Copilot Cowork
- Desktop + shell + browser action -> Microsoft Scout
- Custom workflows and integrations -> Copilot Studio agents

3. Add explicit caveats:
- Mark preview capabilities clearly
- Avoid implying GA if source says preview

## Deliverable Format

1. Main output: index.html
2. Optional: brief README with presenter notes
3. Include a final slide with:
- Key takeaways
- Recommended first pilot
- Source links
