# Part 1 — The ideas (read this first)

**[Ayobami Akinlolu-ojo](https://ayobami.ai4africa.app/)** · CTO & Founder · [AI4Africa](https://ai4africa.app)

<a href="https://ayobami.ai4africa.app/"><img src="https://ayobami.ai4africa.app/images/personal_img/coperate-suite-CEO-style.jpg" alt="Ayobami Akinlolu-ojo" width="240" /></a>

You’re in **Citlite**: about **half** the time is **ideas** (this doc), then about **half** is **hands-on** — **z.ai**, quick checks, and a **live URL** (Vercel or Netlify).

**The flow in one drawing:** open [citlite-visual.excalidraw](citlite-visual.excalidraw) in this repo (Excalidraw.com or the Excalidraw extension in your editor).

Ground rule: the model is a **power tool**. **You** still decide what “good” means.

---

## 1. AI and AI-assisted development

When we say **AI** here, we mean software that handles tasks that need **judgment**: classify something, generate text or code, suggest a next step. In real products it’s almost always **one piece** of a bigger system — not a replacement for your database, your rules, or your judgment.

An **LLM** predicts the next tokens (words, code) from context. It’s **strong** at drafts, variations, scaffolding, and explanations. It’s **weak** as a **source of truth** for prices, legal facts, private data, or “what definitely happened” unless something else verifies it.

**AI-assisted development** means you use models to **move faster** on drafting and exploring — but **you** still set requirements, run the build, read errors, and choose what ships. If money, safety, or reputation is on the line, **you validate** model output.

One line to remember: *the LLM is like a very fast intern — great at volume, risky if you skip review.*

---

## 2. Automation vs agent-style

- **Automation:** fixed path — something happens → known steps → result. Clear rules, predictable.
- **Agent-style:** a loop — look at the situation → plan or use tools → act → look again. Flexible, but you need guardrails (logging, human review, limits).

Most real products are **mostly automation plus validation**, with **small** agent-style loops only where you can handle mistakes. Vibe sessions often **feel** like chatting with an agent, but **your spec and your checks** are what keep the work honest.

---

## 3. What software engineering actually is

**Software engineering** is not “typing code.” It’s turning a problem into something **others can run, trust, and change**:

- **Requirements / acceptance criteria** — “done” in words you could test.  
- **Design** — what talks to what, who owns which data.  
- **Implementation** — code, config, migrations.  
- **Verification** — run it, break it, fix it; automated tests when the team agrees they’re worth it.  
- **Delivery** — deploy, watch it, roll back if needed, document.  
- **Truth and policy** — permissions, facts in a database or contract — not “whatever the model said.”

**Vibe coding does not replace this.** It changes **where many keystrokes come from**. If you skip criteria, review, and shipping discipline, you get **fast junk** instead of **fast progress**.

---

## 4. What is vibe coding?

**Vibe coding** is using AI to **move quickly** from a rough idea to working software — prompts, edits, short loops — while **you** still own the **spec**, the **quality bar**, and **shipping**. It is **not** “turn your brain off.” It’s **think → describe → generate → inspect → fix**.

**Why people say “vibe coding” now**  
The phrase spread after **Andrej Karpathy** talked about it publicly (**2025**). The **habit** is older: Stack Overflow and copy-paste → **Copilot-style** completions → **chat with whole files** → **agent-style IDEs** (Cursor, Windsurf, …) → **builders** that spit out full UIs. The name stuck because teams needed words for “I’m not writing every line by hand.”

**How people actually use AI to write code today**

1. **Assisted typing** — suggestions while you type; you still drive structure.  
2. **Chat + context** — paste errors, ask for refactors; you steer file by file.  
3. **Agent in the repo** — multi-file edits, tests, terminal; you review diffs.  
4. **Builders / UI generators** — fastest way to a **surface** (landing, dashboard shell); you check UX, copy, and whether you can **own the export**.

In Citlite we lean on **(4)** for speed. **(2)** and **(3)** are what you reach for when the product gets serious.

---

## 5. How vibe coding and engineering fit together

- **Vibe** = **how fast you loop** with AI.  
- **Engineering** = **discipline** — criteria, truth, verification, ownership.

They are **not** opposites. People who vibe well **write specs first**, **define done**, and **know when to stop** generating and start **designing systems** (APIs, auth, data, monitoring). Weak work is **prompt → hope → ship**.

---

## 6. Bad habits vs good habits

**Avoid**

- Prompts with **no** acceptance criteria (“make it nice”).  
- Treating the model as **truth** for business or security.  
- **No** phone check, **no** link check, **no** basic accessibility pass — only “looks OK on my laptop.”  
- Putting **API keys or secrets** in front-end code (fine for a toy demo; **not** for real users).  
- Using a **builder** for a problem that really needs a **custom backend** and pretending that won’t bite later.

**Do**

- **Spec before prompt:** role, goal, constraints, format (and examples when it helps).  
- **Iterate with evidence:** try v1 / v2 / v3; compare outputs.  
- **Match tool to phase:** builder for **discovery** and **demos**; repo + tests for **long-term** ownership.  
- **List honest limits:** what this stack **can’t** do yet (auth, webhooks, server-side AI, roles, …).

---

## 7. Three kinds of tools (don’t memorize brands)

- **AI app builders** — fastest MVP and demos; harder when logic and long-term maintenance get heavy.  
- **UI-first generators** — sections, components, landing shells (**z.ai** is in this bucket for our lab).  
- **IDE / agent tools** — real repos, refactors, tests, production-shaped work.

Pick the tool for the **phase**: idea → shipped product → system you maintain.

---

## 8. What you’ll do next

After these ideas, you **build**: a clear **spec**, a page in **z.ai**, a short **QA** pass, then **Vercel or Netlify** so you have a **URL**. The goal is a **link** plus **one clear sentence** about where a **builder stops** and **engineering** has to take over.

---

## The six-step loop (bookmark this)

1. Define the outcome.  
2. Write constraints.  
3. Generate a first version.  
4. Test and inspect.  
5. Refine prompts or patch the work.  
6. Write down decisions and limits.

The classic mistake: **prompting without acceptance criteria**.
