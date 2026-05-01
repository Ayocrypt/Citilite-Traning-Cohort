# Citlite — Theory (compact, public session)

**Citlite** is a **standalone** session: one arc from **clear outcome → shipped static page**. It borrows **a small slice** of how you teach paying cohorts (vibe coding discipline, builder vs engineering limits) — **not** the full depth, syllabus, or artifacts they pay for.

## 1. What you are really teaching

- AI can **speed up** a first UI, but **you** still own the spec, checks, and what gets published.
- **Vibe coding** here means: fast iteration **with** acceptance criteria — not “prompt and hope.”
- One sentence outcome for the room: **“I can describe done, generate a draft, check it like a human, and put a static URL on it.”**

*(Internally you may map this to your longer foundation + prototype weeks — **do not** hand attendees that map or file paths.)*

## 2. Vibe coding (short loop you can show)

A practical loop (you can show 4 steps on screen; full six is optional in prep only):

1. Define outcome (what “done” means).  
2. Write constraints (audience, sections, tone, mobile).  
3. Generate with AI (**z.ai** or any similar UI generator you prefer).  
4. Test and refine (device, links, copy, one basic a11y sanity check).  
5. Optional fifth beat: name **one** thing this stack cannot carry into real prod without engineering.

Anti-pattern to name: **prompting without acceptance criteria**.

## 3. Generate: z.ai (or equivalent)

**z.ai** (or backup tool) fits **fast landing / sections / copy**. Free tiers and UIs change — verify export and whether learners can **own the code** going forward.

## 4. Ship: Vercel and Netlify

Static-friendly hosts: **Git → build → URL**, or upload **dist**. Pick **one** platform in session so the pattern sticks.

Teaching line: real apps with secrets and server logic belong **behind an API** — this hour stays **static-only** on purpose.

## 5. Success criteria for the hour

Learners leave having:

- Stated **one outcome** and **three checks** for a tiny page.  
- One generated UI + **one** honest QA pass.  
- **One** deploy path understood + **one** honest “where a builder stops.”

---

*Diagrams:* optional subtle org watermark (e.g. top-left **AI4Africa**) in `citlite-visual.excalidraw` — match whatever you use in other public assets.
