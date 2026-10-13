# DigiGlobal × VYBE × MINE × Juice Bigfellow × IDC — Release Build

**Built:** October 10, 2026. **Status:** Locally tested release candidate. NOT live-deployed.

This package **extends the user's latest DigiGlobal × MINE Software 3.0 deploy bundle**, preserving its real portfolio images/videos, working MINE diagnostic, downloadable tools and existing test suites.

## First preview

```bash
cd site
npm test
npm run dev
```
Open http://127.0.0.1:4173/launch/ . Test the production form at `/partners/`. The local developer server stores test submissions in `.dev-data/inquiries.jsonl` only on your computer; it sends nothing externally.

## Public page map

| Route | Purpose |
|---|---|
| `/` | Existing DigiGlobal portfolio and original video gallery |
| `/mine/` | Existing MINE asset grading + download operations |
| `/launch/` | Cohesive five-brand public launch |
| `/partners/` | Serious project/budget qualification and real working intake UI |
| `/release/` | Six feed graphics, six Story graphics, six captions and silent teaser MP4 |
| `/juice/` | Real existing audience hub and IDC series routing |
| `/idc/` | Existing IDC series + confirmed official rental booking URL |
| `/release/budget-planner.html` | Internal interactive budget draft + JSON download |
| `/release/content-evidence-ledger.csv` | Data-first media tracker with paid/rights statuses set to unverified |

## Deploy to Cloudflare Pages

1. Use `site/` as **Pages project root** (the existing MINE/portfolio is already designed for that environment). Include `/functions/`.
2. Provision Cloudflare D1 and execute `schema.sql` on the D1 DB. Bind the database as **DB** in the Pages Functions environment. Do this for preview and production.
3. Optional lead alert email: add environment variables `RESEND_API_KEY`, `NOTIFY_FROM` (verified sender address) and `NOTIFY_TO` (your actual receiving inbox). No credentials are in this package.
4. Point your selected domain to the deployment and test all routes, real production inquiries, notification delivery, viewability and provider link permissions. No data is saved in Cloudflare before DB binding.
5. Publish your privacy/retention policy and Terms; finalize absolute OpenGraph links, production UTM tags, talent/music rights, any claims and invoice/checkout links. Configure spam protection/Cloudflare Turnstile for public scale.
6. Test actual VYBE/IDC links from your mobile phone. Links point to existing official websites and do **not** imply you can control those websites from this package.
7. After approval, upload feed/Story cards and captions using your social scheduling tool; there is **no social auto-posting** in this package.

## Reality checks

- VYBE public programming exists, but no reliable verified stream audience, eligible ad inventory or payouts have been proven in this package.
- Instagram's two large *Grid* Reels had suspicious views-to-reach/engagement consistency; no claim of 100K organic unique viewers should be made without the Meta Ads analysis.
- The IDC series **already runs on Juice Bigfellow**. This bundle preserves that distribution identity rather than treating it as a future launch.
- Budget bands are planning examples, not price guarantees; productions require confirmed chain of title, music licenses and talent releases.
- MINE's AI operator, real CRM, external payment processing and multi-tenant software are **not** built by this bundle. The existing deterministic diagnostic, user downloads, full portfolio video modal, public preview pages, and local intake service are implemented and tested.

## Technical QA performed

- 13 automated Node.js tests passed (MINE assessment + API, lead validation, Cloudflare D1 handler).
- Previewed the public release pages with Chromium at 1440px and 390px; no horizontal overflow or missing poster images.
- HTTP status 200 for `/`, `/mine/`, `/launch/`, `/partners/`, `/release/`, `/juice/`, `/idc/` and media previews; lead form local submission created a server-side record.
- Silent vertical teaser MP4 generated from the same release art; publish only after review.

## Asset ownership and publishing

Owner-supplied pictures, posters and videos are inherited from earlier DigiGlobal/IDC/MINE artifacts. Rights to third-party talent likeness, media footage and music must be independently cleared for additional advertising, broadcast or platform monetization. No rights transfer is implied by including the files.
