# Statement of AI Use

**Project:** VENU — Festival Companion (multi-device UX)
**Course:** Human-Computer Interaction · Year 2026
**Author:** [your name here]
**Date:** May 2026

---

## 1. Scope of AI assistance

AI tools were used as a **drafting and acceleration partner** for the digital deliverables of this project, primarily for:

- Writing the HTML / CSS / JavaScript of the three high-fidelity prototypes (mobile, MR headset, smartwatch).
- Drafting supporting documents in the same visual style as the prototypes (personas, style guide, storyboards, user flows, sitemaps, low-fi sketches, user guide).
- Translating and clarifying assignment requirements.
- Code review and refactoring (e.g. adding a pannable AR world to the MR headset prototype, fixing minor bugs).

**All design decisions, research conclusions, and the project's value proposition originate from the author.** AI was used as a writing/coding assistant — not as a design authority. Every output was reviewed, edited, and integrated by the author.

---

## 2. AI tools used

| Tool | Vendor | Purpose |
|---|---|---|
| **Cursor IDE** (with Claude Sonnet / Claude Opus / GPT-class models) | Anthropic / OpenAI via Cursor | Generating prototype code, debugging, refactoring, writing documentation |
| **Web research** via the same chat | mixed | Verifying CSS techniques (drag-to-pan, backdrop-filter, conic gradients) |

No image-generation AI was used — all visuals are hand-coded SVG / CSS.

---

## 3. How AI was used — concrete examples

### 3.1 Prototype generation
Each high-fidelity prototype began with a detailed prompt describing the persona, the platform, the screens, and the visual language. The AI generated the first draft (HTML + CSS + JS in a single file). The author then:

- Reviewed each generated screen against the storyboard.
- Adjusted copy, color, and layout for consistency.
- Requested targeted iterations (e.g. *"add a panoramic world that the user can drag-to-look-around like the mobile map"*).
- Verified the interactions in the browser.

### 3.2 Sample prompts

> **Prompt — initial VR prototype:** "Create a prototype-vr.html similar in spirit to the mobile prototype, but for a pair of VR/AR glasses. Same VENU branding (purple/pink/cyan, dark background). The headset should be drawn around a visor that hosts ~8 HUD screens: Boot, Pair, HUD Home over a festival scene, Radar, AR Navigation, Activity Alert, AR Portal, Settings. Include a bottom dock to switch between screens, status bar, and a toast system."

> **Prompt — drag-to-look feature:** "User feedback says the VR prototype would feel more interactive if the AR scene could be dragged with the mouse, similar to the festival map in the mobile prototype. Wrap the festival scene + AR labels in a wider panoramic world (2400×430) and let the user drag the visor to pan it. Keep HUD overlays (greeting, status bar, dock, side cards) head-mounted. Add a heading compass strip that rotates as the world pans."

> **Prompt — documentation pass:** "Generate a personas.html, style-guide.html, storyboards.html, userflows.html, sitemaps.html, sketches.html, and user-guide.html — all in the same dark VENU visual language as the prototypes. Three personas (Alex 24 / Maria 19 / Dan 32), one user flow per device, one sitemap tree per device, six storyboard panels per device, low-fi paper-style sketches."

### 3.3 What I changed manually

- Persona ages, names, locations, devices owned, and bio details were tuned to fit the Romanian festival context (Electric Castle, UNTOLD).
- Storyboard wording and emotional tags were rewritten in my own voice.
- The style guide color hex values were locked to the brand palette I had already chosen before prompting.
- Several CSS animations (compass spring-back, drag hint timing) were tuned manually after testing.
- The questionnaire data (research tactic #2) was collected by me via Google Forms — AI did not generate the responses.

---

## 4. Limitations & verification

- **Code correctness** — every prototype was opened in the browser and tested click-by-click; any broken interaction was fixed by re-prompting or hand-editing.
- **Visual consistency** — colors, spacing, and typography were cross-checked against the style guide.
- **No hallucinated facts** — venue names, persona biographies, and research statements were either based on real research data I collected or clearly fictional (sample) data labelled as such.
- **No external assets** — all icons are inline SVG; all images are CSS / SVG. There is no risk of unattributed third-party content.

---

## 5. Conversation references

The primary chat used to build this project is preserved inside the Cursor agent transcripts of the workspace. Selected conversation summaries:

- **Initial VR prototype creation** — see commit *"Add VR glasses prototype"*.
- **Drag-to-look upgrade** — see commit *"Add pannable panoramic AR world"*.
- **Documentation batch** — see commit *"Add personas, style guide, storyboards, flows, sitemaps, sketches, user guide"*.

If the evaluator requests a live demonstration of how prompts were issued, I can replay the workflow on demand.

---

## 6. Declaration

I confirm that:

1. AI tools were used **transparently and ethically** as productivity aids.
2. The **final design decisions, evaluation, and synthesis are my own**.
3. All AI-generated content was **reviewed, edited, and integrated by me** before submission.
4. No part of this submission was wholesale copied from another student, public repository, or undisclosed source.

— **[your name here]**
