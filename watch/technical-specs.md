# Starlink Watch — Technical Specification & Manufacturing Brief

**Document Type:** Technical Specification / Manufacturing Brief for factory quoting and prototyping
**Prepared for:** Watch manufacturer, China
**Revision:** 1.0 (Draft — pending factory confirmation of tolerances, tooling feasibility, and movement sourcing)
**Governing doc:** [`starlink-watch-vision.md`](starlink-watch-vision.md) — read for design rationale; this document is the buildable spec derived from it.

**Status note, read first:** this brief translates an approved design direction into real dimensions, materials, and tolerances for an initial quoting and prototyping conversation. Several items are flagged throughout as needing factory engineering input before they're locked — this is a starting brief, not a finished production spec. Section 13 consolidates the highest-risk open items.

---

## 1. Project Overview

A mechanical wristwatch: Apple Watch-proportioned squircle case (45 × 38mm), hand-wound movement visible through both a partially open dial and a full sapphire caseback, sterling silver or warm stainless steel case, quick-release strap pins. Three hands only (hour, minute, seconds) — no date, no complications.

## 2. Case — Dimensions & Tolerances

| Parameter | Spec | Tolerance |
|---|---|---|
| Case height (12–6 axis) | 45.0mm | ±0.10mm |
| Case width (9–3 axis) | 38.0mm | ±0.10mm |
| Case thickness (total, crystal to caseback) | 12.0mm target | ±0.15mm |
| Lug width (strap attachment) | 22.0mm | ±0.05mm — this tolerance is tighter than the case body because it directly affects quick-release pin fit (Section 10) |
| Lug-to-lug drop / strap clearance | TBD — confirm against selected strap materials in `starlink-watch-vision.md` Section 7 | — |
| Crown tube outer diameter | TBD, standard for winding-stem gauge selected (Section 9) | ±0.05mm |
| Case wall thickness (side) | 1.8–2.2mm, material-dependent (Section 12) | ±0.10mm |

## 3. Case Corner Geometry — Critical Spec, Not a Simple Radius

The brief calls for the *exact* Apple Watch silhouette, and the corner geometry is the detail most likely to get this wrong if under-specified. Apple's "squircle" corner is a **continuous-curvature profile (a superellipse/G2-continuous spline)** — the curvature changes smoothly around the corner rather than transitioning abruptly from a flat edge into a constant-radius arc the way a standard machined "rounded corner" does. A simple circular fillet at ~8.5mm radius will produce a case that reads as a generic rounded square, not the specific Apple Watch profile — visually close but recognizably wrong side-by-side.

**Requirement:** the corner profile must be supplied to the factory as a **CAD file (DXF/STEP) with the full curvature spline**, not as a single radius value in a spec table. This is a CNC/wire-EDM tooling question the factory's engineering team needs to confirm feasibility and cost on — flag explicitly during the quoting call rather than assuming standard round-corner tooling will suffice.

## 4. Movement Requirements

**Type: hand-wound (manual), not automatic.** This is the approved direction from `starlink-watch-vision.md` and is restated here as a hard requirement, not a preference — an automatic rotor would both push case thickness past the 12mm target (rotors typically add 2–4mm) and physically block the open caseback view, defeating the "visible from the caseback" requirement outright.

**Recommended base caliber:** Unitas/ETA 6497–6498 architecture, or — since this is sourcing from a Chinese manufacturer — the **Tianjin Seagull ST36 series**, which is built to the same architecture and is a well-established, locally available option worth quoting first for cost and lead-time reasons.

| Parameter | Spec |
|---|---|
| Diameter | 36.6mm |
| Height | ~4.5–5.0mm (confirm exact figure against the specific reference variant selected) |
| Beat rate | 18,000 vph (2.5Hz) |
| Power reserve | ~45 hours (stock) |
| Running seconds position | 6 o'clock (native to this architecture — this is *why* this movement family was selected, not an afterthought) |
| Jewel count | Stock count for selected reference (confirm with supplier); no reduction acceptable if it affects the visible bridge jewels, since jewels are part of the visual "precision" story through the open aperture |

**Visible bridge finishing:** required, front and back. Bridges visible through the open dial aperture and the full sapphire caseback must carry decorative finishing — Geneva stripes (côtes de Genève) and/or perlage (circular graining) on flat bridge surfaces, polished bevels on bridge edges. This is a **non-stock modification** — confirm with the movement supplier or a subcontracted finisher whether this is available as a factory option on the ST36/6497-6498 family or requires a separate finishing vendor relationship.

**Selective skeletonizing — scope note:** only the bridges falling within the open dial aperture's footprint (roughly the 4–8 o'clock zone — see Section 6) need openworking/cutaway treatment. The bridges under the solid upper dial do **not** need to be skeletonized, only decoratively finished, since they won't be visible through the dial (they will be visible through the caseback, where finishing alone is sufficient — no cutaway needed on that side). This keeps the modification scope smaller and cheaper than a full skeleton movement. Confirm with the movement/finishing supplier which specific bridges (mainspring barrel bridge, train wheel bridge, balance cock) fall in the aperture zone for the selected caliber variant, since bridge layout differs slightly between suppliers.

## 5. Movement-to-Case Mounting — Round Movement, Square Case

The movement (36.6mm round) does not natively fit a rectangular squircle case interior — this requires a **casing ring** (also called a movement ring or movement holder): a component machined round on the inside (to the movement's exact diameter, holding it snugly and centered) and shaped to the case's inner squircle profile on the outside, seating and centering the movement correctly under the dial and crown position.

- **Material:** for a serviceable, premium piece, a machined brass or steel casing ring is recommended over the more common injection-molded plastic (Delrin/POM) casing ring used in lower-cost watches — brass/steel holds tolerance better over repeated service openings and matches the "built to last, not to be disposable" posture of the rest of this brand.
- **Critical constraint:** the casing ring's profile near the 6 o'clock zone (where the open dial aperture is) must stay clear of the sightline into the movement, or be finished/blackened neatly if any edge is unavoidably visible — a sloppy casing-ring edge peeking into the open view would undercut the entire point of the design. Flag this specifically to the case engineer; it's an easy detail to overlook since casing rings are normally a fully hidden component.
- **Movement retention:** small movement-holding clamps, screwed into the casing ring from the case sides, secure the movement in place. Confirm clamp positions don't intrude into the open aperture's visible field.

## 6. Dial Construction — The Open Section

The dial is a **partial plate**, not a full circular dial with a cutout — it covers only the top ~58% of the movement (roughly 12 o'clock through 9 and 3, arcing over the top), leaving the bottom ~42% (centered on 6 o'clock) entirely open with no dial material present at all.

- **Cut edge:** the boundary between dial and open aperture is a single shallow, asymmetric curve (see `starlink-watch-vision.md` Section 2 for the design rationale) — like the case corner in Section 3, this curve must be supplied to the dial manufacturer as a **precise CAD/vector file**, not a verbal or approximate description, so the laser-cut or stamped edge matches the intended silhouette exactly.
- **Dial feet:** standard 6497/6498/ST36 dials use dial feet (small locating pins) positioned assuming a full circular dial. Because this is a partial dial, feet positions must be **re-engineered to fall within the remaining solid (upper) portion only** — this is custom tooling, not a stock dial modification, and needs sign-off from whoever manufactures the dial blank.
- **Surface treatment:** Cloud Ivory dial finish (matte, non-metallic) on the solid portion; applied (not printed) markers at 12, 1, 2, 3, 9, 10, 11 per the vision doc, in brushed silver matching the case.
- **What's visible in the open zone:** balance wheel, escapement, and part of the going train — the same bridges called out for decorative finishing in Section 4.

## 7. Crystal Specification

- **Material:** sapphire crystal (scratch-resistant; standard for this quality tier).
- **Shape:** matches the case's squircle profile (Section 3) — **not a standard round crystal blank.** Sapphire crystal suppliers typically stock round blanks and tool custom shapes to order; a squircle crystal requires dedicated tooling and should be flagged as a cost/lead-time item during quoting (see Section 13).
- **Profile:** slight dome or flat — flat is the lower-risk/lower-cost starting recommendation given the crystal is already a custom shape; a domed custom-shape crystal compounds the tooling complexity.
- **Coating:** anti-reflective (AR) coating on the underside is functionally important here, not just a premium nicety — the open aperture's entire purpose is visibility into the movement, and uncoated crystal glare would work directly against that. Confirm whether AR coating on both sides or underside-only is the better cost/performance tradeoff with the crystal supplier.

## 8. Hands — Manufacturing Notes

(Design intent fully specified in `starlink-watch-vision.md` Section 4; this section covers only what a factory needs to build them.)

- Hour and minute hands: open-worked/skeletonized batons, brushed silver finish matching the case, sized to the selected movement's hand-fitting spec (confirm arbor/pipe dimensions against the chosen caliber).
- Seconds hand: fine needle hand, Starlink Emerald finish (confirm colorfast method — anodizing or a durable lacquer, not paint that can chip), small heart-shaped counterweight tail. Mounts to the movement's seconds pinion at the 6 o'clock position per the caliber's native architecture.

## 9. Crown & Stem

- **Position:** upper-right case edge, matching the reference silhouette.
- **Winding stem:** standard gauge for the selected caliber family (confirm exact stem spec with movement supplier) — this determines the crown tube bore diameter in Section 2.
- **Crown shape:** cylindrical, deep coin-edge fluting (deeper than a typical smooth digital-crown-style knurl, since this crown needs real functional winding grip).
- **Crown detail:** blind-debossed heart-and-chain-link mark on the outer face — confirm minimum feature size the crown manufacturer's tooling can hold at this small scale before finalizing the artwork.
- **No second pusher/button** — single crown only, per the approved direction. Do not default to adding a second case-side component to match the reference silhouette; there's no function for it.

## 10. Quick-Release Strap Pin Specification

**Mechanism: generic quick-release spring bar** — not a replica of Apple's proprietary lug-slot band-attachment system. This was an explicit decision in `starlink-watch-vision.md` Section 7 (worth restating here so it isn't silently reinterpreted during tooling): the goal is *tool-free, one-handed strap swaps*, achieved through a widely used, non-proprietary mechanism already standard across the watch industry, not a specific copy of Apple's mechanism.

| Parameter | Spec |
|---|---|
| Spring bar diameter | 1.8mm |
| Spring bar length | 22.0mm (matches lug width, Section 2) |
| Material | Spring-tempered stainless steel |
| Release mechanism | Single-flange quick-release tab (thumb-actuated collar/lever at one end retracts that end of the bar for tool-free removal) |
| Lug hole diameter | 1.85mm (spring bar diameter + running clearance) |
| Lug design requirement | Drilled through-holes at both lugs, **plus a small access clearance cut on the inner lug face** so a thumb or fingernail can reach the release tab — this is a specific lug geometry requirement, not just a hole spec, and needs its own engineering pass given the squircle case's lug shape differs from a standard round-watch lug this spec is normally applied to |

## 11. Water Resistance — Target & Correction of an Earlier Assumption

**Correction from the vision document:** `starlink-watch-vision.md` framed the open dial aperture itself as a water-resistance risk. On closer technical review, that's not quite right — the **dial sits inside the case, under the crystal**, so a hole in the dial doesn't create a new path for water ingress; the crystal-to-case gasket and the caseback-to-case gasket are what actually determine water resistance, exactly as on any watch with a solid dial. The dial aperture is a visual design element, not a sealing surface.

The real water-resistance constraints on this piece are the same ones any square-cased mechanical watch has to solve:
- **Crown seal** is the primary weak point on any mechanical watch (it's the one dynamic, moving seal) — a gasketed crown tube and crown are required regardless of target rating.
- **Square/rectangular case gaskets are inherently harder to seal reliably than round ones** — a round o-ring achieves even compression naturally; a square gasket has to hold consistent compression around four corners, which is a real, independent engineering challenge tied to the case shape itself (see Section 13).

**Recommended target: 3 ATM (30m) — splash, rain, and hand-washing resistant, not swim-rated.** This is a realistic, achievable target given the case geometry and crown-seal constraints, and is consistent with what a piece worn for its mechanical/visual character (not as a dive or sport watch) actually needs. A higher rating is possible but adds cost and complexity disproportionate to how the watch will actually be used — flag as a discussion point if a higher target matters for other reasons.

## 12. Case Material Notes

Both options per `starlink-watch-vision.md` Section 1 (925 sterling silver, satin/unlacquered; warm satin-finished 316L stainless steel) — one manufacturing note worth flagging here that the vision document didn't cover:

**Sterling silver is meaningfully softer than stainless steel**, which matters specifically at two wear points: the caseback screw-down threads (opened/closed at every service) and the crown tube threads (engaged constantly during winding and setting). Repeated wear at these points on a pure-silver case could loosen tolerances faster than on steel over the watch's service life.

**Recommendation for the silver case option:** consider a **hybrid construction** — sterling silver case body and bezel (all visible, patina-eligible surfaces) with a steel caseback-thread insert and steel crown tube (hidden reinforcement points, not visible surfaces). This preserves the full silver patina story everywhere it's actually seen while protecting the two components most exposed to mechanical wear. Flag to the case engineer as an option to quote alongside the pure-silver build.

## 13. Critical Technical Challenges — Consolidated

The highest-risk items across this brief, gathered in one place for the factory quoting conversation:

1. **Squircle corner geometry (Section 3)** — requires CAD/spline data, not a radius spec; confirm CNC/EDM tooling feasibility and cost.
2. **Round movement in a square case (Section 5)** — casing ring engineering, with the added constraint that it must stay invisible within the open aperture's sightline.
3. **Custom partial dial with re-engineered feet (Section 6)** — non-stock dial tooling.
4. **Selective bridge decoration/skeletonizing (Section 4)** — needs a movement finishing vendor relationship, likely outside the base movement supplier's stock offering.
5. **Custom squircle sapphire crystal (Section 7)** — round-blank tooling doesn't apply; dedicated crystal tooling, cost and lead-time impact to be quoted separately.
6. **Square-case gasket sealing (Section 11)** — inherently harder than round-case sealing; achievable at the recommended 3 ATM target but should not be assumed "solved" by copying round-case gasket specs.
7. **Lug quick-release access geometry (Section 10)** — the squircle case's lug shape isn't a standard round-watch lug, so the thumb-access clearance cut needs its own engineering pass rather than reusing an off-the-shelf lug spec.
8. **Sterling silver wear at service points (Section 12)** — recommend the hybrid steel-insert construction rather than treating this as solved by material choice alone.

## 14. QC Checklist

| Check | Tolerance |
|---|---|
| Case overall dimensions | Per Section 2 table |
| Corner profile match to reference CAD | Visual + CMM (coordinate measuring machine) comparison against approved spline, tolerance TBD with factory |
| Lug width / spring bar fit | 22.0mm ±0.05mm |
| Crystal fit / gasket seat | No visible gap, confirmed water-resistance test at 3 ATM per unit or statistical sample (confirm factory's standard QC sampling rate) |
| Dial cut-edge alignment to case | ±0.15mm, dial aperture centered relative to case squircle profile |
| Movement decoration (Geneva stripes/perlage) | Visual inspection against approved reference sample |
| Crown winding/setting function | Full wind and time-set cycle test, every unit |
| Hand alignment (all three hands at 12) | ±1 minute visual alignment at assembly |

## 15. Open Items for Factory Conversation

- Confirm exact reference movement variant (Seagull ST36 sub-variant, or ETA/Unitas sourcing if available) and current lead time/MOQ.
- Confirm feasibility and cost of selective bridge skeletonizing + decoration — in-house capability vs. third-party finishing subcontractor.
- Confirm CNC/EDM tooling cost and lead time for the squircle case profile (Section 3) and squircle crystal (Section 7) — these are likely the two largest tooling-cost line items in the whole quote.
- Confirm casing ring material recommendation (brass/steel vs. standard plastic) and cost delta.
- Confirm gasket engineering approach for the square case at the 3 ATM target (Section 11), and get a real quote/timeline for water-resistance testing.
- Confirm sterling silver vs. hybrid steel-insert construction cost delta (Section 12) before finalizing the silver case option.
- Request a running prototype/proof-of-concept quote before any production tooling commitment, given the number of non-stock components in this build (dial, crystal, case, movement finishing all require custom tooling simultaneously).
