# Packaging Technical Specification — Manufacturing Brief

**Document Type:** Technical Specification / Manufacturing Brief for factory review and costing
**Prepared for:** Shenzhen packaging factory
**Revision:** 1.0 (Draft — pending factory confirmation of tolerances, tooling costs, and Pantone matching)
**Governing docs:** [`philosophy.md`](philosophy.md), [`outer-box.md`](outer-box.md), [`internal-layers.md`](internal-layers.md), [`personal-touch.md`](personal-touch.md), [`sensory-details.md`](sensory-details.md)

**Status note, read first:** every dimension, GSM, and tolerance below is a considered starting spec based on standard rigid-box packaging practice — none of it has been sampled or physically confirmed yet. Treat this as the brief for an initial costing and sampling conversation with the factory, not a locked production spec. Exact Pantone matches, tooling die costs, and MOQ-dependent decisions need factory input before anything is finalized.

---

## 1. Project Overview

A rigid two-piece setup box packaging system for the Chaos Incorporated wardrobe (five SKU-size tiers) and a separate small-format box for Starlink One and future fine jewelry. Full design intent and reveal sequence are documented in the governing docs above — this section is the condensed brief a factory-facing contact needs without reading the full philosophy chain:

- Rigid two-piece box (base + lid), soft-touch matte exterior, rounded corners, ribbon closure (no magnets, no snap-fit hardware).
- No plastic components anywhere in the package — this is a hard requirement, not a preference (see Section 6).
- Color and finish draw from an existing 9-color brand palette (Section 7) and a "silver hardware only" rule already used across the rest of the product line.

## 2. Product Category & Box Dimension Matrix

All dimensions are internal box dimensions (L × W × H), with the ~12–15mm tissue clearance from `outer-box.md` already factored in. Garment folded-size assumptions are approximate and should be confirmed against actual folded samples once available.

| Category | Example Products | Internal Dimensions (mm) | Notes |
|---|---|---|---|
| Folded top | Basics/intricate tops | 260 × 200 × 60 | Single interleaving tissue fold |
| Folded bottoms | Jeans, leggings, shorts, trousers | 320 × 240 × 70 | Slightly deeper for denim bulk |
| Folded outerwear | Jacket, cardigan, vest | 380 × 300 × 90 | Deepest tier for the standard line |
| Dress (flat-pack) | Ring statement dress | 400 × 300 × 50 | Wide/flat rather than deep — tissue rolls (not folds) at the fold line to prevent creasing across the bodice/skirt seam |
| Fine jewelry / ring | Starlink One and future pieces | 90 × 90 × 40 | Separate small-format box, insert cushion TBD pending ring mount design |

## 3. Outer Box Construction

- **Core:** rigid chipboard/greyboard, target thickness 1.5–2.0mm (~1500–2000 gsm equivalent), wrapped construction (not printed folding carton).
- **Exterior wrap paper:** dyed matte stock, 128–157 gsm, finished with soft-touch (velvet) matte lamination film, target 1.0–1.5 mil.
- **Interior wrap paper:** same weight/finish family as exterior, contrasting color per Section 7.
- **Corner radius:** 3mm, all exposed corners on base and lid.
- **Lid depth:** approx. 25–30% of total box height (standard setup-box proportion) — confirm against factory's standard tooling before requesting a custom ratio.
- **Lid fit:** light friction fit only — see Section 9 for the removal-force tolerance. Explicitly **not** a vacuum/telescoping tight fit; over-tight fit produces the "pop" sound this brief is designed to avoid.
- **Target empty-box weight:** 180–260g depending on size tier (Section 2).

## 4. Print & Finish Specs

- **Exterior wordmark:** blind deboss (no ink, no foil), centered on lid top. Deboss depth target 0.3–0.5mm — confirm against board thickness and factory tooling minimums.
- **Heart + chain-link motif:** companion blind deboss, lower corner of lid, single small mark (not a repeat pattern). Approx. 15–20mm at longest dimension.
- **Optional silver foil accent:** confined to the heart shape only, within the motif deboss — combination foil-on-deboss finishing. Flag to factory as a potential tooling/cost adder versus deboss-only; confirm feasibility and MOQ impact before committing.
- **Ink (where used — tissue print, care card, note card):** soy-based or water-based ink only, no solvent-based ink, consistent with the no-plastic/sustainability posture in Section 6.
- **Color matching tolerance:** ΔE ≤ 2.0 against approved physical swatch, once swatches are confirmed (see Section 7).

## 5. Closure Hardware

- **Ribbon:** grosgrain, 10–12mm width, color per Section 7 (Blush Mauve default, Starlink Emerald for gift-tier orders).
- **Attachment:** threaded through two slits cut into the box base (slit width to match ribbon width plus ~1mm clearance), no adhesive attachment — ribbon must be replaceable/re-tieable without residue.
- **Length:** sufficient for a full wrap around the closed box plus a bow, approximately 2.2–2.5× the box's girth (L+W+L+W) — exact length to be confirmed per box size tier.
- **Pull-test tolerance:** ribbon and slit construction should withstand a straight pull of at least 15N without tearing the slit or fraying the ribbon edge (standard handling force, not a stress spec).
- **No magnetic or mechanical closure hardware** — explicitly excluded per `philosophy.md`/`outer-box.md`; do not substitute a magnet or snap without a documented design change.

## 6. Interior Components

| Component | Material | Spec |
|---|---|---|
| **Tissue paper** | Acid-free tissue | 17–20 gsm (mid-weight — avoid the thin/crinkly extreme below ~14gsm), color per Section 7, single spot-color custom print (heart/chain-link repeat, small scale, tone-on-tone) |
| **Note card** | Cotton-fiber or soft-touch matte stock | ~250–300 gsm, A6 (105 × 148mm), letterpress or blind deboss for fixed copy, blank space reserved for handwriting |
| **Care card** | Same stock family as note card | Slightly smaller than the note card for visual hierarchy — exact size TBD, content pulled per-SKU from existing item documentation (see `personal-touch.md`) |
| **Scent card** | Absorbent uncoated card substrate | Fragrance load per IFRA guidelines, hypoallergenic formulation required, must ship as a **separate, removable insert** — never sprayed on or embedded in garment tissue or the garment itself |
| **Dust bag** | 100% cotton or non-woven fabric, ~120 gsm | Drawstring closure (cotton cord, not plastic aglets), small debossed or embroidered motif, sized per category to loosely fit the folded garment |
| **Seal sticker** | Paper stock, matte finish | ~30mm diameter, removable/residue-free adhesive, heart or chain-link motif, **paper only — no plastic film sticker stock** |

**Hard requirement, no exceptions:** no PE film, no cellophane, no bubble wrap, no plastic poly bags, and no plastic-based adhesive tapes anywhere in the package. This is a sustainability and brand-feel requirement simultaneously (see `philosophy.md` Section IV) — flag any factory-standard component that defaults to plastic (e.g., a poly dust-cover bag) for a fabric/paper substitution before sampling.

## 7. Color & Material Palette Reference

Pulled directly from the wardrobe's existing [`color-system.md`](../wardrobe/color-system.md) — packaging introduces no new colors.

| Element | Color Name | Approx. Hex | Pantone Match |
|---|---|---|---|
| Box exterior | Cloud Ivory | `#F5F1E8` | TBD — confirm against factory's physical Pantone bridge book |
| Box interior (default) | Blush Mauve | `#D9A9A8` | TBD |
| Box interior (seasonal alt.) | Sage | `#9CAF9A` | TBD |
| Ribbon (default) | Blush Mauve | `#D9A9A8` | TBD |
| Ribbon (gift-tier alt.) | Starlink Emerald | `#0F5C3D` | TBD |
| Foil/hardware accent | Sterling silver | — | Matte silver foil, standard factory library, confirm finish sample |

**Pantone matching note:** hex values above are digital-screen approximations of the existing brand palette; they are not yet mapped to verified Pantone TPX/TCX codes. Do not proceed to production-run ink mixing from the hex values alone — a physical swatch/Pantone bridge match with the factory is required before finalizing.

## 8. Sustainability & Safety Requirements

- FSC-certified (or equivalent) paperboard and tissue stock.
- Soy-based or water-based inks only.
- Zero single-use plastic components (see Section 6 hard requirement).
- All adhesives residue-free and removable (seal sticker, any tape used in assembly).
- Fragrance components IFRA-compliant and hypoallergenic-formulated; scent card shipped separately from garment-contact materials (see Section 6).
- Dust bag and ribbon are both reusable/washable — no components designed for single use where a reusable alternative is reasonable.

## 9. QC Checklist

| Check | Tolerance |
|---|---|
| Box squareness (base and lid) | ±1.0mm across diagonal measurement |
| Corner radius | 3mm ±0.3mm |
| Lid fit — removal force | Light friction fit; target range 3–8N (deliberately gentle — see `sensory-details.md`, this is not a vacuum-fit spec) |
| Color match (exterior, interior, ribbon) | ΔE ≤ 2.0 against approved swatch |
| Print/deboss registration | ±0.5mm |
| Deboss depth | 0.3–0.5mm, consistent across production run |
| Ribbon slit pull-test | Withstands 15N straight pull without tearing |
| Empty box weight | Within ±10% of the target range per size tier (Section 3) |

## 10. Open Items for Factory Conversation

- Confirm rigid-box tooling lead time and die cost per size tier (Section 2) — five SKU tiers likely means five separate die sets unless tiers can share a base die with depth variation.
- Confirm whether combination foil-on-deboss finishing (Section 4) is standard capability or requires additional tooling/cost.
- Confirm Pantone bridge matching process and physical swatch turnaround (Section 7).
- Confirm MOQ per component (box, ribbon, tissue, cards, dust bag) — packaging MOQs are often higher than garment MOQs and may be the actual constraint on order volume, not garment production.
- Confirm fabric/paper substitution options for any factory-standard plastic components (Section 6) and associated cost delta.
