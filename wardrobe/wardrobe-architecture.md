# Wardrobe Architecture

*The category map for the full system. Governed by [`wardrobe-manifesto.md`](wardrobe-manifesto.md); colors pull from [`color-system.md`](color-system.md); every item follows [`item-template.md`](item-template.md).*

---

## The Six Categories

*Originally five — Dresses was added during Phase 3 once a piece existed that didn't fit cleanly under Tops or Bottoms. See the note at the end of that section.*

### Tops (`/tops/`)
Split into three subfolders — originally two, matching the manifesto's soft/structure duality; `shirts/` was added afterward once a piece existed that was neither a plain basic nor a romantic intricate detail:
- **`basics/`** — solid tees, tanks, long-sleeves, base layers. Quiet, high-rotation, mostly Cloud Ivory / Sterling Grey / Midnight Navy. These exist to be layered under or paired with an intricate piece — they are not where the whimsy lives. **Built: 6 items.**
- **`intricate/`** — the LoveShackFancy x Target DNA: puff-sleeve blouses, smocked bodices, lace-trim camisoles, ribbon-tie necklines, ruffle detailing. This is where Blush Mauve, Periwinkle, and Lavender Mist do the most work. Every intricate top needs the manifesto's "one hard detail" — a structured cuff, a corseted or smocked bodice panel, a substantial (not flimsy) base fabric under any lace. **Built: 10 items**, including the puff-sleeve blouse and smocked top named in the Core Aesthetic Vision.
- **`shirts/`** — button-front woven shirts: an oversized flannel and a camp-collar print shirt. Neither is a quiet basic (both carry real pattern/print) nor a romantic intricate detail (no lace, ruffle, or smocking) — they're their own register, casual-with-personality rather than whimsical. This is also where the color system's print exception gets its most explicit workout: the camp-collar shirt is a deliberately re-colored "cool-toned Hawaiian" print (Starlink Emerald/Sage/Periwinkle) rather than the traditional warm red-orange-gold register, so it stays inside the brand's cool-undertone palette instead of importing a clashing print wholesale. **Built: 2 items.**

### Bottoms (`/bottoms/`)
The most built-out category — see [`bottoms/bottoms-priority.md`](bottoms/bottoms-priority.md) for the full ranking. Seven subfolders: `jeans/` (10), `leggings/` (8), `shorts/` (8), `trousers/` (2), `joggers/` (1), `skirts/` (1, Experimental), `overalls/` (1, Experimental) — skirts and overalls graduated from "no dedicated folder yet" once their first Experimental bet landed.

### Outerwear (`/outerwear/`)
**Built: 6 items.**
- **Structured layers** — cropped denim jacket (Phase 1), lightweight trench (Phase 2), hardware-detailed moto jacket (Phase 3 statement, chain-link trim in silver only per the color system).
- **Soft layers** — chunky knit cardigan (Phase 1), quilted vest (Phase 2, soft-technical).
- **Romantic layers** — kimono duster (Phase 2) — the outerwear subcategory pulling most directly from the LoveShackFancy reference.

### Shoes (`/shoes/`)
**Built: 6 items + the Anchor Heel line.** Every one fit-checked against a 63" frame (heel height changes leg-line math more at this height than at a taller one, so it's documented per item, not assumed):
- **Everyday flats** — ballet flat (Phase 1).
- **Sneakers** — clean sneaker (Phase 1), the "quiet structure" workhorse, same logic as the straight-leg jean.
- **Boots** — heeled ankle boot (Phase 1), knee-high boot (Phase 2).
- **Heels** — block heel pump (Phase 3 statement, 2.5–3", rare-occasion); [`anchor-heel/`](anchor-heel/) "Anchor One" (Must-Have, 2.0–2.25", everyday) — two genuinely different heels serving different jobs, not a duplicate. The Anchor Heel is the moderate-heel-worn-often piece this category's own README argued was the better investment, built out with its own full vision doc and manufacturing brief given how deep the spec runs (3 variations, dedicated tech pack).
- **Sandals** — ribbon-tie sandal (Phase 2), seasonal and romantic.

### Accessories (`/accessories/`)
**Built: 6 items.** This category carries the most direct Starlink One integration in the whole system:
- **Layering jewelry** — sterling silver layering necklace/bracelet set (Phase 1), a heart-emerald statement pendant (Phase 3 fine jewelry) — chain-link detailing and stone color are deliberate callbacks to the ring's own design. This is where the ring gets "matched," not competed with.
- **Hair** — ribbons and silk scrunchies (Phase 2) — a signature LoveShackFancy x Target detail category, pulling heavily from Blush Mauve/Lavender Mist/Periwinkle.
- **Belts** — chain-link belt (Phase 2) — the single most direct hardware echo of Starlink One available in the accessories category.
- **Bags** — everyday crossbody bag (Phase 1, neutral colorway) before any statement bag.
- **Scarves** — everyday silk scarf (Phase 2), styling flexibility (neck, bag, hair).

### Dresses (`/dresses/`)
**Added during Phase 3.** A dress replaces both a top and a bottom at once and doesn't belong filed under either — this category exists because the Phase 3 build plan called for "a statement romantic piece built specifically to showcase the ring," and that piece turned out to be a dress. **Built: 1 item** — the ring statement dress. Stays intentionally small; this is occasion dressing, not everyday rotation.

## Full Looks (`/full-looks/`)
Not a garment category — this is the assembly layer. **Built: 3 looks**, spanning Phase 1 (two everyday looks) through Phase 3 (one statement going-out look), each documenting a complete outfit and checking it against the color system and the ring.

## Cross-Category Rules

1. **Every item lives in exactly one category/subcategory folder** and follows the priority tiers in [`priority-system.md`](priority-system.md).
2. **Color choices default to the 9-color palette** in `color-system.md` unless the item is explicitly an Experimental/Phase 3 bet.
3. **Hardware is silver-family only**, system-wide — this is a hard rule, not a per-item judgment call, because it's what keeps every accessory compatible with Starlink One by default.
4. **Fit rules from the manifesto apply everywhere**, not just bottoms — rise/inseam gets the most explicit treatment because bottoms was built first, but sleeve length, hem length, and proportion-to-63" apply with equal rigor to tops, outerwear, and dresses when that category is built.
