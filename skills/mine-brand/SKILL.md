---
name: "mine-brand"
description: "Enforce the MINE brand identity on anything an LLM builds — ivory/black/gold luxury system in two registers (ivory MINE master, dark Rōnin cinematic), the real wordmark, Julius's actual photo assets, and brand verbiage. Use when building MINE-branded assets so the model stays on-brand, focused on the build, and synced with his real materials instead of stock, repeats, or inventions."
license: "Proprietary — Julius Twum / Digiglobal Media Group"
metadata:
  version: "1.1.0"
  author: "MINE"
compatibility: "Any Agent Skills–compatible system (Claude Code, Cursor, Codex, Copilot). Image/video generation tools needed for visual assets."
---

# MINE Brand

## Purpose
Translate the MINE brand onto any asset being built, keep the LLM focused on the BUILD (not descriptions of the build), and synchronize with Julius's real internal assets. This skill is the brand-enforcement layer — it sits above the other MINE skills.

## When to use
- Any request for MINE-branded output: social posts, pages, merch, decks, video bumpers, banners, quote graphics.
- Any time the model is about to invent branding, reach for stock, or describe instead of build.
- Alongside mine-hooks / mine-repurpose / mine-visibility when the output must look like MINE.

## The brand (tokens)
- **Colors:** ivory/cream `#FAF6EC`, black `#17130F`, gold `#C9A227`. Muted text `#6F685E`.
- **Type:** serif display headlines (luxury voice), letterspaced uppercase kickers. Never geometric-sans headlines — that's the competitors' uniform.
- **Motifs:** thin double gold rules framing panels, triple vertical gold bars (III) top and bottom, gold rule dividers.
- **Wordmark:** black geometric "MINE", gold "I", "E" as three bars. In `assets/mine-wordmark-transparent.png` — **never retype or redraw it.**
- **Voice:** origins yet tech — gold-rush discipline, new-machine leverage. Full verbiage in `references/verbiage.md`. Tagline: **"Mined, not made."**

## The two registers (read this before the competitor check)
MINE speaks in two registers. Both are MINE. MINE is always the master brand — the wordmark (gold "I") stays dominant in both.

1. **Ivory register (the house).** Ivory publishing-house luxury. Cream backgrounds, black type, gold rules. Default for: the book, the system page, community surfaces, anything that teaches or sells. Aesthetic in five words: *ivory publishing-house luxury, not dark SaaS.*
2. **Rōnin register (the cinema).** The thin world — vast darkness, quiet gold, apparitions emerging from black. Serif display, a whisper of gold, defined by what isn't there. For: the Golden Rōnin story-world, cinematic campaign content, warrior-philosophy transmissions. MINE presents it — open with "MINE PRESENTS", keep the wordmark visible, never let the cinema swallow the house.

**Choosing:** teaching/selling/community → ivory. Story/myth/campaign cinema → Rōnin. When in doubt, ivory — the house is the default.

## Build-focus directives
1. **Build the thing, don't describe it.** If asked for a social post, produce the image/HTML. Never deliver a paragraph about what the asset would look like.
2. **Lead with the asset.** Explanation after, one line max — the way Julius works: show it, then talk.
3. **Verify before delivery.** Check the render the way he would: no blanks, no dead media, no garbled text, no repeated photos. If it fails, fix it — don't ship it.
4. **One job per output.** Don't bundle five assets into one mushy deliverable.

## Asset sync rules (hard)
1. **Real assets only.** Pull from `references/asset-manifest.md`. If an asset is missing on this machine, name it — never substitute stock or AI-generated filler.
2. **Julius is never AI-generated.** Real photos only. Never the same photo twice on one surface.
3. **Spec is never client work.** The robot-arm/on-set shots are crew/spec — caption as on-set work, never as commissioned projects.
4. **The book is a hero object.** Physical-feeling, centered, never a thumbnail.
5. **Register check.** Ivory register going dark-tech SaaS (near-black bg, neon accent, geometric sans headlines, no wordmark) → wrong, invert back to ivory/gold/serif. Rōnin register going generic dark (no gold whisper, no serif, MINE swallowed or missing) → wrong, restore the thin world: vast black, quiet gold, wordmark present. Dark is sanctioned only as Rōnin — cinematic, ancestral, MINE-presented.

## Portability (new system setup)
The bundled `assets/` and `references/` are Julius's real materials. On another user's system, replace them: drop their wordmark into `assets/`, their photo manifest into `references/asset-manifest.md`, their verbiage into `references/verbiage.md` — the skill's rules then enforce *their* brand the same way. The two-register structure (house + cinema) ports as-is; rename the cinema register to fit their world.

## Workflow
1. Identify the asset type and surface (social, page, merch, video).
2. Load brand tokens above + verbiage for the words.
3. Pull the real assets from the manifest — wordmark file, the right photo(s), the right template.
4. Build it.
5. Run the verify pass: brand tokens correct, no repeats, no stock, no invented facts, text spelled right.
6. Deliver the file/asset first, one line of context after.
