# 🛡️ HALO Ops

**Human Authority Layered Oversight**: a 7-layer reference model for running AI with a human in the loop.

> The human decides. The AI handles the admin. Together it's one cohesive effort.

**Live site:** https://jsmokeyscott-pixel.github.io/halo-ops/

---

## What it is

There's no OSI-style model for human-AI oversight. Existing frameworks such as in/on/out of the loop, the Sheridan–Verplank levels of automation and the Parasuraman stages describe *how much* a system is automated. They don't say *who owns what* at each step of an operation. HALO fills that gap.

Humans hold **both ends** of the stack. They set the walls at Layer 1 and keep authority at Layers 5–7. The AI works in the middle, inside limits set by people and below a ceiling people control.

| # | Layer | Owner | AI may | AI may never |
|---|-------|-------|--------|--------------|
| 7 | **Command** | Human | Flag conflicts with intent | Set intent or own the outcome |
| 6 | **Decide** | Human | Recommend options | Choose for the human |
| 5 | **Authorize** | Human | Request approval | Self-approve or act without approval |
| 4 | **Execute** | AI (overseen) | Execute approved actions | Expand scope or ignore an abort |
| 3 | **Analyze** | AI (overseen) | Assess and recommend | Act on its own findings |
| 2 | **Collect** | AI (overseen) | Gather and organize | Reach outside approved sources |
| 1 | **Bound** | Human | Work inside limits | Modify its own access |

**Cross-layer rails** (these run through every layer):
- **Cease-fire:** any authorized human can halt any layer, at any time, immediately.
- **Audit:** every request, approval, action and result gets logged. If it isn't logged, it didn't happen.
- **Escalate:** uncertainty, irreversibility and scope changes go *up* the stack. They never get pushed through.

**Layer 5 is the firewall.** Nothing irreversible passes from analysis to action without a human approving it.

**Mnemonic (7 → 1):** *Can Doodles Always Eat All Cheese, Buddy?*
Command · Decide · Authorize · Execute · Analyze · Collect · Bound

---

## Features

- **Dashboard:** interactive stack overview and quick-start cards
- **Layers:** step through each layer: human and AI roles, rules, escalation triggers and a net ops example
- **Router:** answer yes/no checks about a task and get **GO / HOLD / CONFIRM / NO-GO**, plus the layer it routes to
- **Drill:** 12 randomized scenarios scored GO/NO-GO against an 80% standard
- **Reference:** quick-reference table, the rails, and how HALO maps to existing frameworks, with print / save as PDF
- Light and dark mode, mobile-friendly, a single self-contained file, no build step

---

## Run it

**Online:** open the live site.

**Locally:** download `index.html` and open it in any browser. It works offline; without internet the custom fonts fall back to system fonts.

## Deploy your own copy (GitHub Pages)

1. Create a public repo named `halo-ops`.
2. Upload `index.html` and `README.md` to the root of the repo.
3. Go to **Settings → Pages**.
4. Under **Source**, choose **Deploy from a branch**, then select `main` and `/ (root)`, and click **Save**.
5. Wait a minute or two. The site appears at `https://<your-username>.github.io/halo-ops/`.

## Using it in a class

- Teach the stack from the **Layers** tab, top to bottom.
- Have students run a real or made-up task through the **Router** and explain the verdict.
- Use the **Drill** as a check on learning. 80% is a GO.
- Print the **Reference** tab as a handout.

---

## Files

```
index.html   # the entire app (HTML + CSS + JS)
README.md    # this file
```

## Version

v1.0 · Concept model and application by Scotty.
