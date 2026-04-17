# An Introduction to the Claude Certified Architect – Foundations (CCA-F)

## ROLE
You are an expert instructional designer and senior front-end engineer. Build a 
single-page educational website that helps a VISUAL LEARNER pass the Claude 
Certified Architect – Foundations (CCA-F) exam by Anthropic. Prioritize diagrams, 
color-coded visuals, flow charts, and interactive elements over dense paragraphs.

## DELIVERABLE
One self-contained HTML file (inline CSS + vanilla JS, or Tailwind via CDN). No 
external build step. Must work offline after the page loads. Mobile-responsive. 
Dark-mode friendly with a toggle.

## EXAM FACTS TO ENCODE (verified)
- Exam: Claude Certified Architect – Foundations (CCA-F) by Anthropic
- Launched: March 12, 2026
- Format: 60 scenario-based multiple-choice questions, 120 minutes, proctored
- Scoring: Scaled 100–1,000; passing score = 720
- Level: "~301-level," assumes 6+ months of hands-on Claude experience
- Fee: USD 99
- 6 scenarios exist; 4 are drawn randomly per exam — study all 6

## FIVE DOMAINS (weights)
1. Agentic Architecture & Orchestration — 27% (heaviest)
2. Tool Design & MCP Integration — ~20%
3. Claude Code Configuration & Workflows — 20%
4. Prompt Engineering & Structured Output — ~17%
5. Context Management & Reliability — ~16%

## SIX PRODUCTION SCENARIOS
- Customer Support Resolution Agent
- Code Generation with Claude Code
- Multi-Agent Research System
- Developer Productivity with Claude
- Claude Code for CI/CD
- Structured Data Extraction

## SITE STRUCTURE (required sections, in this order)
1. HERO — "Your Visual Path to the CCA-F." Show a large animated SVG roadmap 
   with the 5 domains as milestones and a progress indicator.
2. EXAM AT A GLANCE — Dashboard-style tiles (questions, time, passing score, 
   fee, prerequisites). Use icon cards, not paragraphs.
3. DOMAIN DEEP-DIVES — 5 collapsible sections, one per domain. Each must 
   include:
   • A weight donut chart (SVG)
   • A concept map (nodes + edges showing relationships)
   • 3–5 key terms as flashcard flip-tiles
   • A "common traps" panel with red/green visual do/don't examples
4. SCENARIO GALLERY — 6 scenario cards in a grid. Each card expands to a 
   visual workflow diagram (boxes + arrows) showing the ideal architecture. 
   Color-code by primary domains involved.
5. MENTAL MODELS LIBRARY — Visual one-pagers for:
   • Hub-and-spoke orchestration
   • CLAUDE.md hierarchy pyramid (global → project → subdir)
   • MCP primitives triangle (tools / resources / prompts)
   • JSON schema validation retry loop
   • "Lost in the middle" context placement diagram
6. 12-WEEK STUDY PLAN — Visual Gantt-style timeline with checkboxes. 
   Persist checked state in localStorage (note: if deploying where storage 
   isn't available, use in-memory state).
7. PRACTICE QUIZ — 15 scenario-based MCQs with instant feedback, visual 
   explanations (diagrams inside the feedback), and a domain-performance 
   radar chart shown at the end.
8. GLOSSARY — Searchable visual glossary. Each term gets an icon + one-line 
   definition + mini-diagram where applicable.
9. CHEAT SHEET — Printable single-page visual summary of all five domains.

## VISUAL DESIGN PRINCIPLES
- Heavy use of SVG diagrams, flowcharts, and icons
- Every concept must have a visual; text is secondary support
- Consistent color per domain (pick 5 distinct accessible colors)
- Use progressive disclosure: overview first, details on click
- Animations on scroll for diagram reveals (subtle, not distracting)
- High contrast, dyslexia-friendly font (Atkinson Hyperlegible or similar)
- Print stylesheet for the cheat sheet section

## INTERACTIONS
- Sticky left-side nav with domain jumps and progress tracking
- Flashcard flip animations for key terms
- Quiz with timer and scoring visual
- Dark/light toggle
- Search bar that filters glossary and scenarios

## CONTENT DEPTH
For each domain, include:
- Task statements (what you must be able to DO)
- Key knowledge points
- 2–3 worked visual examples
- 1 anti-pattern diagram (what NOT to do)

## TONE & ACCURACY
- Technical but approachable
- Cite the domain weight in each section
- Do NOT invent Anthropic internals — stick to publicly documented behavior 
  of Claude Agent SDK, Claude Code, MCP, and the Messages API
- Flag anything uncertain as "verify with official exam guide"

## OUTPUT
Produce the complete HTML file in ONE artifact, ready to open in a browser. 
Include placeholder SVGs you draw inline — do not link external images.
