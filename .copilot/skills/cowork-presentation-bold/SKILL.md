---
name: copilot-presentation-style
description: 'Create HTML presentation pages in Microsoft 365 Copilot style. Use when user asks for presentation pages, slide-like landing pages, deck-style storytelling, visual sections with 3-box modules, architecture diagrams, platform icons, top navigation bar, and a clear red thread from problem to outcome.'
argument-hint: 'Topic, audience, key message, required sections, and available assets'
user-invocable: true
---

# Copilot Presentation Style

Generate slide-like HTML pages with the exact visual language from this project.

## When To Use

- Build a new HTML presentation page.
- Convert slide content into a web presentation.
- Enforce consistent Copilot brand look across pages.

## Mandatory Design Constraints

- Light warm background only. No dark sections.
- Blue-to-pink gradient treatments for cards, CTAs, highlights, and hover states.
- Always include a top navigation bar with anchors to major sections.
- Keep a clear narrative thread across the page:

  1. Problem
  2. Approach
  3. Proof or impact
  4. Next steps

- Use visual communication heavily in every main section:

  - 3-box modules
  - Architecture visuals or process diagrams
  - Platform icon rows or logo strips

## Required Style Tokens

- Colors: #091F2C #0078D4 #C03BC4 #8661C5 #8DC8E8 #FFA38B #FF5C39 #FFF8F5 #F4F3F5
- Gradient primary: linear-gradient(135deg, #238CD9 0%, #CA6CCD 100%)
- Gradient hover: linear-gradient(135deg, #0078D4 0%, #C03BC4 100%)
- Typography: Segoe Sans Display Semibold (headings), Segoe Sans Display/Segoe UI (body), Arial fallback

## Inputs To Collect

1. Topic
2. Audience
3. Core message
4. Required sections
5. Available media assets (logos, icons, architecture images, screenshots, videos)

If inputs are missing, use [request template(wird in neuem Fenster geöffnet)](https://m365.cloud.microsoft/chat/assets/request-template.md) and ask for only the missing fields.

## Procedure

1. Build the page structure in this sequence by default:

   - Hero
   - Agenda
   - Challenge
   - Solution
   - Demo
   - Impact
   - Next steps

2. Add a fixed top navbar with anchor links for all major sections.
3. Ensure each major section includes at least one visual block.
4. Apply the required design tokens and gradients via CSS variables.
5. Make the layout responsive for desktop and mobile.
6. Verify no section drifts into dark theme styling.

## Output Expectations

- Semantic HTML sections
- Reusable CSS variables
- Accessible image alt text
- High-fidelity presentation polish aligned to this workspace design guide

## Local References

- Main guide: ../../../Design_Guide_Copilot_Presentation.md
- Short prompt: ../../../vibecoding_prompt_short.txt
- Request template: ./assets/request-template.md
