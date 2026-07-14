# Starlink Watch — Foundational Vision Document

*A mechanical watch for the Chaos Incorporated universe. Governed by the same design discipline as [`../wardrobe/wardrobe-manifesto.md`](../wardrobe/wardrobe-manifesto.md) and [`../packaging/philosophy.md`](../packaging/philosophy.md), and built to sit on the same wrist as Starlink One without competing with it.*

---

## 0. Where This Sits in the Universe

Starlink One's whole design argument is a soft shape (the heart) held secure by visible, honest engineering (four prongs, an open gallery setting, an unprotected finish that's allowed to live and change). Starlink Watch takes that exact argument and runs it through a second medium: instead of a stone held by prongs, it's a **gear train held by a case** — and instead of hiding that mechanism behind a solid dial the way almost every watch does, this watch does what the ring already does with its stone: it lets you see the thing that's actually doing the work.

That's the whole concept in one sentence: **a mechanical watch that treats its own mechanism the way Starlink One treats its emerald — as the part worth showing, not hiding.**

## 1. Case

### Silhouette & Dimensions

The brief for "exact silhouette and proportions of an Apple Watch" is a real, specific geometry, not a vibe — a rounded-rectangle ("squircle") case, taller than it is wide, with continuous-curvature corners rather than simple circular-arc corners. Target dimensions, referenced against Apple's well-documented public case specs for their 44–45mm line:

| Dimension | Target | Reference |
|---|---|---|
| Case height | 45.0mm | Matches Apple's 45mm case height |
| Case width | 38.0mm | Matches Apple's case width at this height tier |
| Case thickness | 11.5–12.5mm | See thickness note below — mechanical movements need more depth than a quartz/battery stack |
| Corner radius | Continuous-curvature squircle, ~8.5mm effective radius | Not a simple round-cornered square — the corner curvature needs to *accelerate* smoothly the way Apple's does, or the silhouette reads as a generic rounded square instead of the specific Apple Watch profile |
| Lug width (strap attachment) | 22mm | Standard for the 44–45mm Apple Watch tier |

**Thickness honesty check:** Apple's 45mm case is ~10.7mm thick, which is achievable for quartz but tight for mechanical. A thin hand-wound movement (see Section 3) can realistically get total case thickness to **11.5–12mm** — close enough that the silhouette reads as correct at a glance, without pretending a real balance wheel and gear train fit in a quartz-thin case. An automatic movement with a rotor would push this to 14mm+ and visibly break the proportions; this is the main reason Section 3 recommends hand-wound as the primary spec, not automatic.

### Material Options

Both options stay inside the system-wide "silver hardware family only" rule from [`../wardrobe/wardrobe-architecture.md`](../wardrobe/wardrobe-architecture.md) — no gold or warm-toned metal anywhere on this watch, ever.

**Option A — Sterling Silver (925), flagship option.**
Same metal, same alloy, as Starlink One itself — this is the most direct material continuity available. Finished satin/brushed (not mirror-polished) for a diffuse, warm light response rather than a cold hard glint. Left **unlacquered and unprotected**, exactly like the ring — the case is expected to oxidize and develop patina at the same rate and character as Starlink One, so a watch worn daily on the same wrist as the ring will visibly *age together* with it. This is the single most on-brand material decision available for this piece, and it's a real point of difference from virtually every commercial watch, which is built specifically to *resist* the thing this brand wants to happen.

**Option B — Warm Stainless Steel, everyday option.**
316L stainless, satin/brushed finish (same "warm" logic as the wardrobe copy uses — warm refers to a soft, diffuse, matte-leaning finish quality, not a warm metal tone; this stays firmly in the cool, silver-toned hardware family). More durable and lower-maintenance than sterling silver for daily wear; does not patina the way the silver option does, so it's the pragmatic choice for someone who wants the silhouette and openness story without the ongoing tarnish-care conversation.

**Recommendation:** ship Option A as the flagship/statement piece (the one that's *actually* paired with Starlink One in marketing and full-look styling) and Option B as the everyday-durable variant — the same Must-Have/Statement logic the wardrobe's priority system already uses.

## 2. Dial

### The Solid/Open Split

The dial is not skeletonized edge-to-edge — that would read as generic "skeleton watch" rather than a specific, intentional Chaos Incorporated statement. Instead:

- **Top ~58% of the dial** (roughly 12 through 9 and 3, arcing over the top) is a solid dial plate in Cloud Ivory, carrying the hour markers and providing the "at a glance" legibility a watch actually needs.
- **Bottom ~42%** (centered on 6 o'clock) is fully open — no dial plate at all, a true aperture straight down into the movement: balance wheel, escapement, and part of the gear train, all visible and moving.

### Shape of the Open Aperture

The boundary between solid dial and open aperture is **not a straight cut** — a hard horizontal bisection would read as industrial/technical, which fights the "warmth" requirement. Instead, the boundary is a **single shallow, asymmetric curve** — closer to the lower arc of a heart's silhouette than a mechanical dial-cutter's straight line. This is the dial-level execution of the same "soft shape, hard architecture" rule the ring and the wardrobe both run on: the *opening itself* is soft, even though what it reveals underneath is precision engineering.

### Markers & Legibility

Applied (not printed) baton markers at 12, 1, 2, 3, 9, 10, 11 in brushed silver matching the case metal, sized and spaced for real legibility — this is a watch meant to be read quickly, not just admired. No markers at 4, 5, 6, 7, 8 — that entire zone is inside the open aperture and doesn't need them; the exposed gear train does the visual work there instead.

## 3. Movement — Visible From Front *and* Back

**Recommended base caliber: a hand-wound (manual) movement in the Unitas/ETA 6497–6498 family**, or a comparable hand-wound movement of similar architecture. This is a deliberate, specific recommendation, not a placeholder:

- These calibers run **~36.6mm in diameter** — large enough to fill a wide 38mm-wide case properly, so the open aperture reveals a real, substantial mechanism rather than a small movement rattling around in too much case (the exact "swimming in too much space" failure mode the packaging system already flags for boxes — same principle, applied to a movement in a case).
- They're **hand-wound**, so there's no automatic rotor to block the caseback view — the entire back of the movement is visible, sapphire caseback, no exceptions.
- Their **running seconds sits at 6 o'clock** by native architecture — which lines up exactly with the open aperture's center. This isn't a coincidence being engineered around after the fact; it's the reason this specific movement family is the right starting point.
- Commercial skeletonized versions of this movement family already exist, meaning the engraving/openworking vendor relationships and tooling knowledge already exist in the supply chain — a real, practical advantage for a small-batch or indie production run, not just an aesthetic one.

**Caseback:** full sapphire crystal, no engraving or text obstructing the view — the entire back of the movement, bridges, and mainspring barrel visible, finished with Geneva stripes or perlage on the bridges so what you're looking at is worth looking at, not just functional.

## 4. Hands — Hour, Minute, Seconds Only

No date, no chronograph, no complications beyond timekeeping — the brief calls for exactly three hands, and that restraint is correct for this piece: any additional dial clutter would compete with the open aperture for attention, and the whole point is that the mechanism itself is the "complication" worth looking at.

- **Hour and minute hands:** open-worked (skeletonized) batons in brushed silver matching the case — a thin outlined shape rather than a solid filled hand. This matters mechanically, not just stylistically: both hands sweep through the open aperture's lower half on every rotation, and a solid hand would block the movement view every time it passes through 4–8 o'clock. An open-worked hand lets the movement stay visible even while the hand is crossing it.
- **Seconds hand:** the one hand allowed a color accent — a fine, needle-thin hand in **Starlink Emerald**, pivoting from the true seconds pinion at 6 o'clock (per the movement's native architecture) and sweeping directly over the open aperture. You see the hand *and* the escapement driving it in the same glance — precision and openness, literally in the same field of view. The counterweight tail is a small, quiet **heart shape** — a direct, specific callback to Starlink One, sized small enough to read as a considered horological detail rather than a gimmick (heart-shaped counterweight tails are an established watchmaking convention; this isn't inventing a new mechanism, it's pointing an existing one at the ring).

## 5. Crown Design

- **Position:** upper-right case edge, matching the Apple Watch digital crown's exact position — this is one of the most recognizable silhouette cues of the reference geometry, so it's preserved precisely even though this crown does something completely different (winding and time-setting, not a digital input).
- **Shape:** cylindrical with deep coin-edge fluting — deeper than Apple's knurling, because a mechanical crown needs real winding torque and grip, not just a touch-sensitive surface. This is a case where "exact silhouette" and "actually functional" diverge slightly, and function wins on the fluting depth specifically while the overall position/proportion stays faithful.
- **Detail:** a small blind-debossed heart-and-chain-link mark on the crown's outer face — the one place a finger touches this watch most often, carrying the same quiet motif already used on the packaging (see [`../packaging/outer-box.md`](../packaging/outer-box.md)) and worth repeating here for the same reason: a detail felt more than seen.
- **No second pusher/button.** Apple's case has a second button (the side button) below the crown; this watch omits it. There's no digital function for it to trigger, and adding a non-functional second button purely to match the silhouette would be decoration for its own sake — exactly the kind of choice the wardrobe manifesto's "structure earns its place" rule exists to rule out.

## 6. Overall Color Direction

Pulled directly from the existing [`../wardrobe/color-system.md`](../wardrobe/color-system.md) — no new colors invented for the watch, same discipline the packaging system already followed.

| Element | Color | Role |
|---|---|---|
| Dial (solid portion) | Cloud Ivory | Warm, soft, legible base |
| Case & hands (silver option) | Sterling silver, satin finish | Metal continuity with Starlink One |
| Case & hands (steel option) | Warm stainless steel, satin finish | Same finish logic, more durable metal |
| Markers | Brushed silver, matching case | Legibility without introducing a new tone |
| Seconds hand | Starlink Emerald | The single saturated color accent — used exactly once, per the "one loud element at a time" rule already established across the wardrobe system |
| Movement finishing | Natural nickel/rhodium plating, Geneva stripes | Left in its honest mechanical tone rather than colored or dyed — the movement's own material is the "openness" statement, it doesn't need help from color |

## 7. Strap System

### The Quick-Release Requirement — A Note Worth Flagging

"Quick-release strap system exactly like Apple Watch" is a request for a *specific mechanism* (Apple's proprietary lug-slot band attachment), not just an "easy to swap bands" outcome — worth pausing on, because there are two different paths here and they have different implications:

1. **A literal copy of Apple's proprietary lug-slot mechanism** would allow this watch to physically accept the entire existing ecosystem of real Apple Watch bands — a genuinely appealing outcome (huge selection, familiar swap action, no new tooling for straps). The tradeoff: this specific attachment mechanism (not the general concept of a quick-release band) is a distinct, specifically-engineered system, and case shape plus a specific proprietary mechanism together is a more notable thing to reverse-engineer than either alone.
2. **A generic quick-release spring bar** (a widely used, non-proprietary mechanism already standard across dozens of watch brands) delivers the *same user experience* — one-handed, tool-free band swaps — through a different, unencumbered mechanism, at the cost of not being compatible with actual Apple Watch bands.

This document specs the **generic quick-release spring bar** (path 2) as the default recommendation — same ease-of-swap outcome the brief is actually asking for, without the specific-mechanism question. If literal Apple band compatibility is a deliberate goal (not just "easy swaps"), that's a decision worth making explicitly rather than by default, and worth a conversation with whoever handles IP/legal before tooling — flagging it here rather than quietly picking one path for you.

### Strap Materials & Colors — "Warm Hug," Applied to a Band

All strap options use the 22mm lug width from Section 1 and the quick-release mechanism above. Four options, each pulling a different material language already established elsewhere in the system:

- **Soft-touch silicone** — Cloud Ivory, Blush Mauve, or Sage. The everyday-durable option; same "soft, stretchy, extreme comfort" priority named in the original wardrobe brief, applied to a wrist-worn object worn as many hours a day as any garment.
- **Woven textile** — a chunky-knit-inspired braided strap, same material language as the wardrobe's chunky knit cardigan (see [`../wardrobe/outerwear/02-chunky-knit-cardigan.md`](../wardrobe/outerwear/02-chunky-knit-cardigan.md)) — cozy, textured, visibly soft rather than technical.
- **Leather** — soft, vegetable-tanned leather in Cloud Ivory or Sterling Grey, deliberately chosen to patina and soften with wear rather than resist aging — the strap-level execution of the same "wear it in, don't varnish it" rule the silver case option already carries.
- **Chain-link mesh bracelet (statement option)** — sterling silver, matching Starlink One's own chain-link scale exactly, the same "match, don't compete" logic already used for the wardrobe's chain-link belt and layering bracelet (see [`../wardrobe/accessories/03-chain-link-belt.md`](../wardrobe/accessories/03-chain-link-belt.md)). This is the Phase-3-equivalent statement band — lower everyday comfort than silicone or leather, highest direct visual connection to the ring.

## 8. How This Reads as Precision, Warmth, and Openness

Explicit accounting, so the brief's three words are checkable against actual design decisions rather than left as a mood board feeling:

- **Precision:** a real mechanical movement, sized correctly for the case rather than shrunk to fit; applied markers, not printed; a seconds hand that visibly answers to a visible escapement; Geneva-striped movement finishing that rewards close inspection.
- **Warmth:** satin/brushed finishes everywhere, zero mirror polish; Cloud Ivory dial base; a case metal (sterling silver) that's allowed to age and soften over time instead of staying showroom-perfect; soft strap materials (silicone, knit, leather) prioritized over the cold chain-link option as the default.
- **Openness:** the defining structural decision of the whole piece — an honest window into the mechanism, both front and back, with a hand-wound movement chosen specifically because it doesn't hide its own seconds-keeping behind a rotor.

## 9. Open Questions for Next Steps

- **Movement sourcing:** confirm exact base caliber (6497 vs. 6498 vs. an alternative hand-wound movement of similar architecture) and whether openworking/skeletonizing is done in-house, by the movement supplier, or by a third-party engraver.
- **Case tooling:** the continuous-curvature squircle corner is a real CNC/tooling challenge, not a simple round-corner spec — confirm with a case manufacturer before finalizing the corner radius number in Section 1.
- **Quick-release mechanism:** the Section 7 fork (generic spring bar vs. literal Apple-compatible mechanism) needs an explicit decision before lug geometry is finalized, since the two mechanisms may require different lug tolerances.
- **Water resistance target:** not yet specified — an open dial aperture is a real engineering constraint on water resistance (there's no solid dial plate acting as a barrier over part of the movement), and this needs a target spec (likely a modest splash-resistance rating rather than a swim-rated one) before case engineering can proceed.
- **Sterling silver caseback durability:** confirm whether the caseback itself should also be unprotected sterling silver (fully consistent with the case) or a more wear-resistant sapphire-surround in steel even on the silver case option, since the caseback sits directly against skin more than the case sides do.
