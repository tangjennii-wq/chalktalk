# 🎓 Chalk Talk Generator

A free web tool that generates **10-minute board-aligned chalk talks** for internal medicine doctors. Built by Jennifer Tang, MD.

**🔗 Live tool:** [https://tangjennii-wq.github.io/chalk-talk/](https://tangjennii-wq.github.io/chalk-talk/)

---

## What it does

Pick a topic. Pick a mode. Get a structured 10-minute teaching session anchored to current society guidelines and landmark trials in about 30 seconds.

- 🎓 **Lecture Mode** — Physiology-first, mechanism → presentation → workup → management
- 📋 **Boards Mode** — UWorld-style vignette with 5 choices, explanation, and discriminating features

Built around the full ABIM Internal Medicine blueprint. Covers all subspecialties (cards, pulm, GI/hep, endo, ID, heme/onc, nephro, rheum, neuro, ICU, allergy, derm, psych, geriatrics, women's health, prevention, palliative) and is anchored to society guidelines (KDIGO, AHA/ACC, ATS, IDSA, ACG, AASLD, ADA, ACR, AAN, SCCM, ASH, ASCO, AAAAI, AAD, APA, AGS, ACOG, USPSTF, AAHPM).

**Features:** chat-based refinement · AI medical illustrations · podcast audio · peer-review pass for accuracy · optional web search verification · 🚩 disagree-with-answer feedback

---

## Getting started

You'll need a free **Anthropic API key** (~3 min setup):

1. Sign up at [console.anthropic.com](https://console.anthropic.com)
2. Add a payment method (~$5 free starter credits = ~20 talks)
3. Generate an API key
4. Paste it into the tool when prompted

Your key stays in your browser only — never sent anywhere except Anthropic. Each generation costs roughly **$0.10–$0.30** in API charges, billed to your own account.

---

## How it works

This is **prompt engineering with structured output** — not RAG. It uses a carefully designed system prompt that constrains Claude to behave like an experienced IM educator. Three accuracy layers run in sequence:

1. **Chain-of-thought generation** (Claude Sonnet 4) — explicit step-by-step reasoning before writing
2. **Optional web search** — verifies current society guidance from PubMed, NEJM, society pages
3. **Silent peer review pass** (Claude Haiku) — a second model reviews for factual errors and silently revises if needed

The user only sees the final, reviewed output.

---

## Disclaimer

This is a **teaching tool**, not a clinical decision support system. AI-generated content should be reviewed by a qualified physician before use. Board questions are AI-generated, not pulled from licensed question banks — best used as discussion starters, not as a substitute for official board prep.

---

## License

Released under [**CC BY-NC-SA 4.0**](https://creativecommons.org/licenses/by-nc-sa/4.0/) — free for educational use with attribution. Commercial use prohibited. See [LICENSE](./LICENSE) for full terms.

---

## Contact

**Jennifer Tang, MD** · Internal Medicine, Nephrology · [LinkedIn](https://www.linkedin.com/in/tangjennii/)

If you're an educator using this tool, I'd love to hear what's working and what's missing. Open an issue or reach out directly.

---

*A teaching tool, free for educational use.*
