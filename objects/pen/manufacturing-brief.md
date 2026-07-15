# Gallery One — Manufacturing Brief

**Document Type:** Technical Specification / Manufacturing Brief for factory quoting and prototyping
**Prepared for:** Fountain pen manufacturer, Taiwan (TWSBI-adjacent demonstrator/piston-pen specialists) — see Section 7 for why this sourcing region is named specifically rather than left generic
**Revision:** 1.0 (Draft — pending factory confirmation of barrel construction method, window tooling, and piston sourcing)
**Governing doc:** [`vision.md`](vision.md) — read for design rationale; this document is the buildable spec and the language intended to go directly to a factory contact.

**Status note, read first:** this brief translates an approved design direction into dimensions, materials, and tolerances for an initial quoting and prototyping conversation. It is not a finalized production spec — Section 12 lists what needs factory engineering confirmation before tooling begins, and Section 11's ink-contact question (unprotected sterling silver vs. ink) is the single highest-priority item to resolve before Option A is locked as the flagship spec.

---

## 1. Project Overview

A cartridge/converter-compatible piston-fill fountain pen with a true open demonstrator window over the ink chamber and piston (not a peep-hole), a rhodium/palladium-plated steel #6 nib, and a machined chain-link knurled grip section. Screw-cap closure, no posting. Two material options: sterling silver overlay (flagship) or rhodium-plated silver trim over a weighted brass core (everyday/first-prototype default). Sized for a smaller hand — substantial but under full-size (Montblanc 149) territory.

## 2. Barrel & Cap — Dimensions & Tolerances

| Parameter | Target | Tolerance |
|---|---|---|
| Length, capped | 138–142mm | ±0.5mm |
| Length, uncapped (writing) | 125–128mm | ±0.5mm |
| Barrel max diameter | 14–15mm | ±0.2mm |
| Grip section diameter | 10.5–11.5mm | ±0.15mm — tighter than barrel diameter since this directly affects in-hand control, not just fit |
| Cap inner diameter (barrel mating) | Barrel max diameter + running clearance for chosen thread spec (Section 8) | ±0.1mm |
| Weight, capped, filled | 32–38g | — (confirm against Section 12 prototype build; this is an estimate pending physical sample) |
| Balance point (uncapped) | ~20mm forward of grip section midpoint | Confirm via prototype; depends on final piston mass and barrel wall thickness (Section 12) |
| Nib unit | JoWo or Bock #6 housing, standard threaded mount | Confirm housing thread spec matches selected nib supplier exactly — JoWo and Bock #6 units are not universally interchangeable at the threading level despite both being "#6" |

## 3. Barrel & Cap — Material Specification

Both options stay inside the system-wide silver-hardware-family rule (see [`../../wardrobe/wardrobe-architecture.md`](../../wardrobe/wardrobe-architecture.md)) — no gold or warm-toned metal anywhere, including the nib (Section 5).

**Option A — Sterling Silver (925) overlay, flagship.**
- Construction method: confirm with factory whether this is achieved as a **cast/turned solid silver barrel and cap** or a **silver overlay electroformed/soldered over an ebonite or resin core** — both are established sterling-silver-pen construction methods with different cost, weight, and durability profiles, and the vision document does not commit to one. Overlay-over-core is the lighter, more cost-effective route and is the more common approach for silver-bodied demonstrator-style pens in the existing supply chain; solid-turned silver is heavier (helps hit the 32–38g target on its own) but more expensive in raw material and machining time. Get both quoted.
- Surface pattern: machine-turned (engine-turned) or hand-guilloché base pattern, satin finish — **explicitly no mirror polish**, matching the finish rule used across the ring, watch, and wardrobe hardware.
- Finish state: shipped **unlacquered**. Do not apply a clear protective lacquer as a factory-standard "tarnish prevention" default — this is a deliberate brand requirement (the piece is meant to patina), not an oversight to catch in QC.
- **Gating dependency:** do not commit to Option A as the production spec until Section 11's ink-contact question has a factory or materials-lab answer. Flag this explicitly during the quoting call so the factory doesn't proceed on tooling assumptions for a barrel construction that may need a protective treatment near the section threads.

**Option B — Brass core, rhodium-plated silver cap band/clip/nib trim, everyday/first-prototype option.**
- Barrel core: cast brass, weighted to help hit the 32–38g target (brass density is the practical source of the "over-engineered" heft called for in the vision document).
- Trim: sterling silver, rhodium-plated, on the cap band, clip, and nib housing trim only — satin finish, matching Option A's finish rule.
- Ink contact: the brass core does not contact ink or skin directly in this configuration, which sidesteps Section 11's staining question entirely — this is the reason Option B is recommended as the safer first-prototype build regardless of which option ships as the eventual flagship.

## 4. The Ink Window — Manufacturing Spec

- **Position:** spans roughly the rear two-thirds of the barrel, from just behind the grip section back to the piston knob.
- **Material:** optically clear cast acrylic or high-grade clear resin — **not glass or sapphire**. This window is a structural barrel wall under grip pressure during normal handling, not a static cover, so material choice must tolerate that load; acrylic/resin is the standard, well-understood choice in the existing demonstrator-pen supply chain.
- **Wall thickness:** confirm minimum thickness the factory recommends to hold structural integrity under grip pressure and repeated piston-fill handling without an explicit target imposed here — this is a factory engineering call, not a designer-specified number, since it depends on the specific acrylic/resin grade selected.
- **Boundary curve — CAD deliverable, not a verbal spec:** the window's forward edge (where it meets the opaque grip section) is a single shallow, asymmetric curve, not a straight machined cut (see `vision.md` Section 3). Exactly as with the Starlink Watch's case corner and dial cut-edge, **this curve must be supplied to the factory as a CAD/vector file (DXF or equivalent)**, not described in prose or approximated from a sketch — a curve this specific will not survive translation through a factory's own interpretation of "soft asymmetric arc."
- **Seam/joint to opaque grip section and rear barrel:** confirm the factory's standard method for joining a clear window section to opposing opaque barrel sections (threaded joint, adhesive bond, or press-fit) and whether the joint line can be hidden at or near the boundary curve rather than appearing as a visible ring across the barrel.
- **Long-term clarity — open item:** confirm expected UV and age performance (yellowing, hazing) of the specific acrylic/resin grade proposed; this is flagged as unresolved in `vision.md` Section 11 and needs a real answer, not an assumed "acrylic is fine" default, before this window material is locked for production.

## 5. Nib — Sourcing & Grind Spec

- **Housing:** JoWo or Bock #6 nib unit — confirm which supplier the factory has an existing relationship with, since switching suppliers later changes housing thread spec (Section 2) and may require a grip-section retool.
- **Material:** stainless steel, rhodium- or palladium-plated. **No solid gold nib option, at any tier** — this is a hard material exclusion carried over from the vision document's silver-only hardware rule, not a cost-driven default; do not offer gold as an upsell option during factory conversations about premium tiers.
- **Grind:** Fine as the standard/default grind for initial production; Medium as a secondary option once Fine is validated. No stub, italic, or flex grinds in the initial spec.
- **Engraving:** fine chain-link mark on the underside of the nib's breather-hole area — confirm minimum feature size the nib supplier's engraving/etching tooling can hold at this scale before finalizing artwork; nib surfaces are small and this detail is easy to lose if under-specified.

## 6. Grip Section — Knurling Manufacturing

The chain-link pattern is cut as functional grip texture, not applied decoration (see `vision.md` Section 5) — this has a direct manufacturing implication: the knurling tooling must produce a pattern fine enough to read as ordinary grip texture from normal viewing/handling distance, resolving into the literal chain-link shape only on close inspection.

- **Method:** fine machined/knurled cut directly into the grip section material (matches barrel material per Option A/B, Section 3) — not a separately molded or applied grip sleeve.
- **Feature size:** confirm with the factory the finest chain-link feature size their knurling tooling can hold while still functioning as effective grip texture (too fine loses grip function; too coarse loses the "resolves into a chain link on close inspection" effect) — this needs a physical sample to validate, not a spec-table number alone.

## 7. Filling Mechanism — Piston Sourcing & Construction

- **Recommended mechanism:** piston-fill system in the **TWSBI/Pelikan architecture family**, named specifically (not left as a generic "piston mechanism" placeholder) because this family is mature, well-documented, and has existing tooling and supplier relationships already active in the pen manufacturing world — the direct reason Taiwan is named as the preferred sourcing region in this brief's header: TWSBI is a Taiwan-based manufacturer with deep, existing demonstrator/piston-pen manufacturing expertise, making a Taiwanese factory relationship a real sourcing advantage rather than an arbitrary regional choice.
- **Confirm at quoting:** whether the piston mechanism itself is sourced as an off-the-shelf component from an existing piston-mechanism supplier, licensed from a TWSBI/Pelikan-family design, or requires custom piston tooling — `vision.md` Section 11 flags this as unresolved, and the cost/lead-time difference between these three paths is large enough to need an answer before any production commitment.
- **Piston knob position & window visibility:** knob sits at the extreme rear of the barrel; full piston travel must be visible through the Section 4 window — confirm the piston rod/mechanism housing itself doesn't obstruct the sightline through the window at any point in its travel.
- **Converter compatibility:** nib housing (Section 5) accepts a standard international cartridge/converter as a secondary fill method. Confirm this doesn't require a different housing spec than a piston-only design would — some piston mechanisms integrate directly into the section in a way that complicates simultaneous cartridge/converter compatibility, and this needs factory engineering input, not just a checkbox spec.

## 8. Cap, Clip & Closure — Manufacturing Spec

- **Closure: screw cap.** Confirm thread pitch and number of turns-to-close with the factory — a screw closure meant to read as "slow and deliberate" (per `vision.md` Section 7) needs a specific turn count (2.5–3 full turns is a reasonable starting target for this size pen) rather than a fast single-turn thread; flag this explicitly since factory-standard fountain pen cap threads vary widely in turn count.
- **No posting:** confirm the cap's inner geometry is not sized/toleranced to grip the barrel's rear end, since that end is occupied by the piston knob (Section 7) and the hidden cabochon detail (Section 9) — a posting-compatible cap would risk marking or obscuring both.
- **Clip:** leaf-shaped, spring-tensioned, sterling silver (Option A) or rhodium-plated silver (Option B), satin finish matching the barrel. Confirm spring tension target with the factory against a comparable reference clip (e.g., a TWSBI or similar mid-weight pen clip) rather than leaving tension unspecified — too loose fails its clipping function, too stiff damages pocket/bag fabric over repeated use.
- **Clip underside detail:** small blind-debossed heart-and-chain-link mark, positioned to sit against the cap when clipped (hidden in normal wear). Confirm minimum debossing feature size the factory's tooling can hold at clip scale.

## 9. Starlink One Reference — Manufacturing Notes

- **Piston knob cabochon:** small heart-cut synthetic emerald or emerald-toned resin cabochon set into the flat rear face of the piston knob. Confirm setting method (bezel-set vs. bonded/adhesive-set) given the knob is a handled, rotating component subject to repeated grip contact during filling — a setting method adequate for a static surface may not hold up to that handling, and this should be tested on the first prototype rather than assumed.
- **Piston seal accent:** fine ring of Starlink Emerald-tinted material (`#0F5C3D` per [`../../wardrobe/color-system.md`](../../wardrobe/color-system.md)) on the piston head, visible only through the Section 4 window during travel. Confirm with the piston supplier whether their standard seal material (typically a synthetic rubber/silicone compound) can be color-matched to this hex reference directly, or whether a custom-tinted seal batch is required — this is a small-volume custom color order and should be flagged for lead-time impact during quoting.
- Confirm both details are invisible on the capped, at-rest pen — no exterior emerald color and no chain-link hardware visible at rest, per the "discovered, not advertised" rule already applied to the ring, watch, and Anchor Heel.

## 10. Color & Finish Specification

Pulled directly from [`../../wardrobe/color-system.md`](../../wardrobe/color-system.md) — no new colors introduced for this object.

| Element | Color / Finish | Hex (where applicable) |
|---|---|---|
| Barrel & cap (Option A) | Sterling silver, satin, unlacquered | — |
| Barrel & cap (Option B) | Rhodium-plated silver trim over brass core, satin | — |
| Nib | Rhodium/palladium-plated stainless steel | — |
| Ink window | Optically clear acrylic/resin, no tint | — |
| Piston knob cabochon & piston seal accent | Starlink Emerald | `#0F5C3D` |
| Grip knurling | Matches barrel material/finish (Section 3) | — |

## 11. Ink-Contact Staining — Highest-Priority Open Question

Restated here from `vision.md` Section 11 because it directly gates Section 3's material recommendation: **confirm with a silversmith or an experienced fountain-pen manufacturer whether normal fountain-pen ink contact (filling, occasional spill, capillary wicking near the section threads) produces graceful, even tarnish on unprotected sterling silver, consistent with the patina story the rest of the system relies on — or whether it produces uneven staining that reads as damage.** This needs a real answer, ideally from someone with hands-on experience finishing silver-bodied pens, before Option A is finalized as the production spec. If the answer is unfavorable, the fallback is not necessarily abandoning Option A outright — a factory-recommended barrier treatment at the ink-contact zone only (section threads, interior barrel wall near the window) while leaving the rest of the barrel unlacquered is worth asking about as a middle path.

## 12. Critical Technical Challenges — Consolidated

1. **Barrel construction method for Option A (Section 3)** — solid-turned silver vs. overlay-over-core; get both quoted, since cost, weight, and durability all differ.
2. **Ink-contact staining on unprotected sterling (Section 11)** — the single biggest open question in this brief; resolve before Option A is locked.
3. **Window boundary curve tooling (Section 4)** — requires CAD/vector delivery, not a verbal spec, same class of risk as the watch's squircle corner and dial cut-edge.
4. **Window material long-term clarity (Section 4)** — confirm UV/age performance before locking the acrylic/resin grade.
5. **Piston mechanism sourcing (Section 7)** — off-the-shelf vs. licensed vs. custom tooling; large cost/lead-time spread between these paths.
6. **Cartridge/converter compatibility vs. piston-only housing design (Section 7)** — confirm this doesn't require a compromised or non-standard nib housing.
7. **Cabochon setting durability on a handled, rotating component (Section 9)** — test on first prototype, don't assume a static-surface setting method holds up.
8. **Custom seal color-matching (Section 9)** — confirm lead time/MOQ for a small-batch custom-tinted piston seal against the `#0F5C3D` reference.

## 13. Requested Next Step

A running prototype in **Option B** (brass core, rhodium-plated silver trim) only, with the Section 4 window, Section 5 nib, and Section 7 piston mechanism all functional, before any commitment to Option A or production tooling. Option B sidesteps the Section 11 ink-contact question entirely, letting the first prototype validate the parts of this brief that are shared risk regardless of final material choice — window boundary tooling, piston sourcing, and cartridge/converter compatibility — the same "prove the shared risk first" logic the Anchor Heel brief applies to its own single-variation first prototype. Once Option B is validated, run the Section 11 ink-contact question in parallel so Option A can be quoted with a real answer in hand, rather than as an open assumption.
