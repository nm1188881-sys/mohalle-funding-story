
## Plan: Mohalle Mastane — Investor Roadmap (Phase 01 cover)

Start with the cover/Phase 01 section now, using the uploaded image as the hero. Subsequent phases will be added as you share each image. Color palette and typography will be locked from this first image (warm cream/sand background, deep charcoal text, serif display + clean sans subheads) and reused across all future phases.

### Scope for this step
1. Upload the provided image as a Lovable asset (so the original quality is preserved and bundle stays light).
2. Replace `src/routes/index.tsx` with a full-screen Phase 01 section:
   - Left column (sticky on desktop): phase number "01", title "Oneness Oasis", kicker "Master Vision", divider, "A Bhoomi of Oneness", short description, and the four pillars (Coexistence, Compassion, Togetherness, Sustainability) with simple line icons.
   - Right column: large image display of the Oneness Oasis render, edge-to-edge on desktop, full-width on mobile.
   - Minimal top brand bar: "Mohalle Mastane" wordmark + subtle "Phase-wise Funding Roadmap" label.
3. Add the three investor fields requested, styled subtly under the description so they don't fight the image:
   - Funding Required — placeholder (e.g. "To be confirmed") until you share the number.
   - Key Objectives — short bullet list seeded from the image's pillars; editable later.
   - Expected Impact — one-line placeholder; editable later.
4. Smooth scroll + snap setup so future phase sections (`<section>` per phase) scroll cleanly. Mobile = stacked, single column; desktop = two-column with sticky text.
5. SEO: route `head()` with title "Mohalle Mastane — Phase-wise Funding Roadmap", matching description, OG/Twitter tags, and the Oneness Oasis image as `og:image`.
6. Design tokens added to `src/styles.css` (cream background, charcoal foreground, muted sand, hairline border) so all future phases inherit the palette automatically — no per-section color overrides.

### Questions before I publish
- I will NOT publish yet. You asked to "upgrade the full website once it's complete with all the pages", so I'll deploy and generate the shareable URL after the final phase is in. Tell me if you'd rather have a live link after Phase 01 too.
- For "Funding Required / Key Objectives / Expected Impact" on Phase 01 — do you want me to leave them as clearly-marked placeholders, or omit them on the cover and only show them from Phase 02 onward? Default: clearly-marked placeholders.

### Technical notes
- Image goes through `lovable-assets create` from `/mnt/user-uploads/…` → `src/assets/phase-01-oneness-oasis.png.asset.json`, imported in the route.
- Icons via `lucide-react` (Users, Heart, Leaf, RefreshCw) to match the line-icon look in the source image.
- No backend, no Lovable Cloud — pure static marketing route.
- Single route file `src/routes/index.tsx`; each future phase becomes another `<section>` in the same file (or a small `PhaseSection` component) so one-page smooth scroll works.

Reply "go" (or with answers above) and I'll build Phase 01. Then send Phase 02's image whenever you're ready.
