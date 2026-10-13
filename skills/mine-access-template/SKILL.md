---
name: "mine-access-template"
description: "Template for a user's unified data-access layer in the MINE Operator — connect your own social and data sources, document the exact pull commands, and name the honest gaps. Use when setting up MINE for a new operator. Fill in the brackets, then rename to mine-access."
license: "MINE template — free to adapt"
metadata:
  version: "1.0.0"
  author: "MINE"
  distribution: "template"
compatibility: "Any Agent Skills–compatible system. Commands adapt to the user's connected tools."
---

# MINE Access — the Embassy (Template)

## Purpose
One skill that groups all of *your* connected data sources. The MINE Operator pulls through here — ingest, then coach, then work. If a source isn't listed as live, don't pretend it is. Fill in every bracket below with your own accounts, commands, and gaps, then delete this paragraph.

## Live sources

### Instagram — [LIVE / NOT CONNECTED]
- Linked account: `[handle]` (account id `[id]`).
- Pull profile: `[exact command]`
- Pull posts/reels: `[exact command]`
- Rate behavior: normal use is fine; don't hammer.

### Email — [LIVE / NOT CONNECTED]
- Via `[skill or tool]`. For monitoring (replies, opportunities), not social metrics.

### [Additional source] — [LIVE / NOT CONNECTED]
- `[what it can pull + exact command]`

## Gaps (documented, not hidden)

### [Source] — [NO CONNECTOR / BLIND SPOT / NOT LINKED]
- What you can't reach and why.
- Workaround: `[how you fill the gap manually]`. Flag it whenever a plan assumes this data.

## Rules
1. **Pull, don't guess.** Every number in the system comes from a command above or a stated manual entry. Fabricated metrics are the one unforgivable sin.
2. **Cache smart.** Metrics change slowly — daily pulls max for scoreboards, weekly for proof. Don't re-pull inside a loop.
3. **Gaps go in the report.** If a source is missing, the output says which one and what it blocks — it never silently substitutes.
4. **Respect the blind spots.** Never claim data from an unconnected source.

## Setup checklist
- [ ] Connect each source through your system's actual flow (don't invent a connection).
- [ ] Verify one real pull per source before marking it LIVE.
- [ ] Write the exact command — copy-pasteable, no paraphrase.
- [ ] Name every gap and its workaround.
- [ ] Rename this skill directory to `mine-access` when it holds real data.
