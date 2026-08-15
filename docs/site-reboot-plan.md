# Site Reboot Plan — The "Grounded Content" Narrative

**Status:** Planning only. No site changes yet. Next step after sign-off: build a local walk-through version.
**Assumption:** Replatform (Multi-Platform Converter, v0.12.0) is **live** at publish time.
**Constraint:** Keep the existing visual style, components, and layout system as-is. This is a *narrative* reboot (message architecture, section order, new-feature sections), not a visual redesign.

---

## 1. Why reboot instead of adding cards

The current site is built on **"Scale LinkedIn Content, Not Your Headcount"** — a *content studio* frame: voice match + volume + seven formats. That was right for the v0.9 product.

Since then the product quietly became something different. Everything shipped after v0.9 points at one theme: YourTake now builds **a living model of everything true about your brand** — how you sound, the stories you've lived, what your customers actually say, the proof you've earned, where you're headed — and generates content that is **grounded, not generic**. With replatform live, that grounded content now goes **everywhere**, not just LinkedIn.

Bolting 6+ new features onto an IA built for the old story produces feature-list soup — the exact "AI slop" problem the product fights. A narrative reboot makes every feature *evidence for one claim* instead of a loose card.

**Positioning principle (from the customer):** the *data we gather is the "how."* We sell what it **unlocks** — content that's unmistakably yours and actually true. We do **not** sell the data itself, and we do **not** coin a category label ("digital twin" etc.). The concrete enumeration is the pitch.

---

## 2. The spine: Know → Create → Everywhere

Input → transform → output. A three-act structure with a short compounding coda.

```
HERO   Content that's unmistakably yours — and actually true. Everywhere.

ACT 1  KNOW        YourTake learns everything true about your brand.
ACT 2  CREATE      Every post is grounded in that truth, in your voice, any format.
ACT 3  EVERYWHERE  One piece, adapted to every platform, ready to post.

CODA   IT COMPOUNDS  The model gets sharper the more you use it.
```

Each act is a claim; each feature is proof of one claim. Nothing floats.

---

## 3. Feature → act mapping (every shipped feature + replatform)

**Legend:** `NEW` = shipped since last site update and not on the site today · `EXISTING` = already on the site · `ENH` = enhancement to something already on the site.

### ACT 1 — KNOW (the living model of your brand)
| Feature | Status | Role in the act |
|---|---|---|
| Voice / Style Guide (built from LinkedIn or website) | EXISTING | The foundation: how you write |
| LinkedIn Post Import → Voice Card + enrichment lanes (pillars, POV, structures, voice drift) | **NEW** | The headliner for Act 1 — voice learned from your *real* posts, not a questionnaire |
| Story Bank / Experience Bank (your lived experiences, via interview or voice capture) | **NEW** | The stories only you have |
| Customer Voice (how your audience actually talks) | EXISTING | What your market says |
| Customer Stories / Customer Proof bank (real outcomes, tagged by ICP) | **NEW** | The proof you've earned — *distinct from Customer Voice* |
| Partners dataset | **NEW** | Who you work with |
| Strategy (goal + audience + POV) | EXISTING | Where you're headed — the directional layer; steers Act 2 |
| Content Library + Discover | EXISTING | Raw source material you feed it |
| Auto-refresh source watcher (weekly delta-crawl + review) | **NEW** | Keeps the model *living* — bridges to the Coda |
| Blog-crawl auto-seeding of story/proof banks | **NEW** | Onboarding accelerant (supporting detail, not a headline) |

> **Careful separation:** Customer Voice (how the audience *talks*) and Customer Proof (verifiable *results*) are two different assets. Keep them visibly distinct — same mistake to avoid as brand-voice vs. customer-voice.

### ACT 2 — CREATE (grounded content, in your voice, any format)
| Feature | Status | Role in the act |
|---|---|---|
| Seven formats (text, carousel, video script, infographic, newsletter, blog, meme) | EXISTING | Range |
| Grounding pickers + provenance badges ("built from your story / customer proof / product") | **NEW** | The visible link back to Act 1 — proof that grounding is real |
| Backwards Science / citation grounding (claim detector → find source → cited swap w/ diff) | **NEW** | Accuracy mechanism (partially implied today by "verified sources") |
| Verified sources / no hallucinated stats | EXISTING | Trust claim (now *backed* by the mechanism above) |
| Custom content styles (your own post/blog/newsletter/carousel structures) | **NEW** | Your structures, not templates |
| Infographic visual styles (12 art directions + Auto + custom) | **NEW** | Visual range |
| Announcement workflow ("Announce") | **NEW** | A grounded create-mode for milestones/funding/launches |
| Promote / "Feature Your Products" workflow | **NEW** | A grounded create-mode for promoting products/partners |
| Variant scoring (quality + voice match) | EXISTING | Best candidate surfaced |
| Conversational refine + split-screen LinkedIn preview | EXISTING | Editing |
| Anti-AI-slop filtering | EXISTING | The "not generic" promise |
| Campaign planning / "Plan Your Month" | EXISTING | Create at the calendar level |

### ACT 3 — EVERYWHERE (distribution)
| Feature | Status | Role in the act |
|---|---|---|
| **Replatform / Multi-Platform Converter** | **NEW (star)** | One LinkedIn piece → X, Facebook, Instagram, Threads, TikTok, YouTube Shorts. Medium-aware, correctly sized, **copy/export only — no auto-posting** |
| Newsletters + Blogs beyond LinkedIn (+ export to any platform) | EXISTING | The original "beyond LinkedIn" surface — now part of a bigger Act 3 |

> **Copy guardrails for replatform:** describe the **text + image** conversion only. The **video-upload path is not built** (blocked on vendor + legal). No claims about posting on your behalf.

### CODA — IT COMPOUNDS (the model gets sharper)
| Feature | Status | Role |
|---|---|---|
| Performance tracking (baseline after 3 posts, per-post scoring) | EXISTING | Learns what works |
| Weekly AI reviews (best format/theme, what to adjust) | EXISTING | Feedback loop |
| Voice learns from your edits | EXISTING | Voice sharpens |
| Auto-refresh source watcher | **NEW** | Sources stay current |

Short closing beat, not a full act — it reinforces "*living* model."

### Intentionally minor / not hero'd (mention only where natural)
Full-Library export/import · Multiple brand logos (up to 5) · Strategy Report · Strategy "start from your notes" · saved directions. These are supporting detail or FAQ-level, not sections.

---

## 4. Homepage section order (proposed)

Keeping existing components/style; re-sequencing and adding new-feature sections.

1. **Hero** — new outcome-led headline (see §6) + primary CTA. Retain existing hero layout.
2. **Act 1 — Know** — lead section: the living model. Voice Card / LinkedIn import as the hook, then a compact visual of the brand assets it learns (voice, stories, customer voice, proof, partners, strategy).
3. **Act 2 — Create** — grounded content + seven formats + provenance badges + the "not generic" promise. Fold Announce/Promote in as create-modes.
4. **Act 3 — Everywhere** — replatform as a distinct, punchy section (this is the new "wow").
5. **Coda — It compounds** — short band: tracking, weekly reviews, learns-from-edits, auto-refresh.
6. **Persona selector** — unchanged (links to the 3 sub-pages).
7. **Pilot / founder-led program** — PRESERVE existing module.
8. **Testimonials** — PRESERVE.
9. **FAQ** — update: keep strong existing entries (ChatGPT, voice, strategy-vs-campaign, pricing), add grounding/accuracy, Customer Proof vs Customer Voice, multi-platform.
10. **Final CTA** — PRESERVE.

**Homepage-thinness fix:** today the homepage renders Campaign / Customer Voice / long-form as thin cards while sub-pages carry the depth. The three-act spine gives the homepage its own real structure without duplicating every sub-page section.

---

## 5. Sub-page approach (agencies / teams / professionals)

Same three-act spine, audience-framed. **Preserve** each page's tested modules — pilot/onboarding, testimonials, and especially the **agency funnel-mapped campaign detail** — and re-spine around them.

- **Know** reframes per audience: agencies = per-client brand models; teams = per-executive models on a company base layer; professionals = your own model.
- **Create** keeps the audience-specific proof already written (agency client sign-off, team coordination, professional anti-repetition).
- **Everywhere** (replatform) is a strong add for all three — one client/exec/personal post → every platform.
- New-feature sections to add where they fit the audience: Story Bank (all three), Customer Proof (all three), Announce/Promote (strongest for teams + professionals; agencies too for client launches), custom styles + infographic styles (agencies especially).

Decision to make later: how much of the depth is homepage vs. sub-page. Default: homepage states each act once; sub-pages carry the deep dives.

---

## 6. Hero direction (straw men — copy is a later pass)

Outcome-led, grounded, multi-platform. Not a coined label. LinkedIn stays the "home base" (voice is learned there; posts start there) but the headline no longer boxes us into LinkedIn-only.

- "Content that's unmistakably yours — and actually true. Everywhere."
- "Every post, grounded in everything true about your brand."
- "Sounds like you. Backed by proof. Ready for every platform."

Sub-head does the reason-to-believe with the enumeration: *"YourTake learns how you sound, the stories you've lived, what your customers say, and the proof you've earned — then turns it into grounded content for every platform."*

---

## 7. What we are deliberately NOT doing

- Not redesigning the visual style, grid, or component system.
- Not coining a category term (no "digital twin").
- Not selling the data collection as the feature — selling the unlock.
- Not marketing the replatform **video** path (unbuilt/blocked).
- Not throwing away converting modules (pilot, testimonials, agency funnel).

---

## 8. Decisions (locked)

1. **Hero lane:** *"Content that's unmistakably yours — and actually true. Everywhere."* Sub-head: *"YourTake learns how you sound, the stories you've lived, what your customers say, and the proof you've earned — then turns it into grounded content for every platform."*
2. **Strategy:** folded into **Act 1 (Know)** as the "where you're headed" layer; noted as steering Act 2. Not a standalone top-level beat.
3. **Depth split:** homepage **states each act once** (crisp); the sub-pages (agencies/teams/professionals) carry the full feature deep-dives.
4. **Coda:** ships as **its own short closing band** ("It compounds") to reinforce the *living* model.

## 9. Build approach

- Build in a local **preview** area served via `python3 -m http.server`; do not touch live pages.
- **Homepage first** as the reference implementation → walk through + iterate → then propagate the spine to the three sub-pages.
- Reuse existing components, grid, and styles. New sections mimic existing section markup/classes.
