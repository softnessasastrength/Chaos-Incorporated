# Wardrobe Architecture

*The category map for the full system. Governed by [`wardrobe-manifesto.md`](wardrobe-manifesto.md); colors pull from [`color-system.md`](color-system.md); every item follows [`item-template.md`](item-template.md).*

---

## The Six Categories

*Originally five — Dresses was added during Phase 3 once a piece existed that didn't fit cleanly under Tops or Bottoms. See the note at the end of that section.*

### Tops (`/tops/`)
Split into four subfolders — originally two, matching the manifesto's soft/structure duality; `shirts/` and `translucent/` were added once pieces existed outside basics/intricate:
- **`basics/`** — solid tees, tanks, long-sleeves, base layers. Quiet, high-rotation, mostly Cloud Ivory / Sterling Grey / Midnight Navy. These exist to be layered under or paired with an intricate piece — they are not where the whimsy lives. **Built: 6 items.**
- **`intricate/`** — the LoveShackFancy x Target DNA: puff-sleeve blouses, smocked bodices, lace-trim camisoles, ribbon-tie necklines, ruffle detailing. This is where Blush Mauve, Periwinkle, and Lavender Mist do the most work. Every intricate top needs the manifesto's "one hard detail" — a structured cuff, a corseted or smocked bodice panel, a substantial (not flimsy) base fabric under any lace. **Built: 10 items**, including the puff-sleeve blouse and smocked top named in the Core Aesthetic Vision.
- **`shirts/`** — button-front woven shirts: an oversized flannel and a camp-collar print shirt. Neither is a quiet basic (both carry real pattern/print) nor a romantic intricate detail (no lace, ruffle, or smocking) — they're their own register, casual-with-personality rather than whimsical. This is also where the color system's print exception gets its most explicit workout: the camp-collar shirt is a deliberately re-colored "cool-toned Hawaiian" print (Starlink Emerald/Sage/Periwinkle) rather than the traditional warm red-orange-gold register, so it stays inside the brand's cool-undertone palette instead of importing a clashing print wholesale. **Built: 2 items.**
- **`translucent/`** — Soft Light tops (sheer long-sleeve base, organza/chiffon blouse, lace panel camisole). Governed by [`translucent-system.md`](translucent-system.md) opacity map — Experimental, not a Phase 1 foundation. **Built: 3 items.**

### Bottoms (`/bottoms/`)
The most built-out category — see [`bottoms/bottoms-priority.md`](bottoms/bottoms-priority.md) for the full ranking. Seven subfolders: `jeans/` (10), `leggings/` (8), `shorts/` (8), `trousers/` (2), `joggers/` (1), `skirts/` (2, Experimental — including Soft Light translucent midi), `overalls/` (1, Experimental).

### Outerwear (`/outerwear/`)
**Built: 7 items.**
- **Structured layers** — cropped denim jacket (Phase 1), lightweight trench (Phase 2), hardware-detailed moto jacket (Phase 3 statement, chain-link trim in silver only per the color system).
- **Soft layers** — chunky knit cardigan (Phase 1), quilted vest (Phase 2, soft-technical).
- **Romantic layers** — kimono duster (Phase 2) — the outerwear subcategory pulling most directly from the LoveShackFancy reference.
- **Soft Light** — sheer organza duster (Experimental) — translucent veil outerwear per [`translucent-system.md`](translucent-system.md).

### Shoes (`/shoes/`)
**Built: the core 8-shoe catalogue + Anchor Heel system + Soft Structure jelly line** (see [`shoes/README.md`](shoes/README.md) for the complete named list). Every one fit-checked against a 64" frame (heel height changes leg-line math more at this height than at a taller one, so it's documented per item, not assumed):
- **Everyday flats** — the Perfect Flat (Phase 1, ballet + loafer hybrid, hidden 0.5" wedge).
- **Sneakers** — the Cloud Walker (Phase 1, elegant-chunky, Gore-Tex option), the "quiet structure" workhorse, same logic as the straight-leg jean.
- **Boots** — the Hug Boot (Phase 1, Chelsea + Western hybrid, chain-link pull tab), knee-high boot (Phase 2), the Rain/Snow Boot (waterproof Chelsea — the one shoe in the whole system where the "moderate heel worn often" rule is deliberately overridden, since ice/wet-weather traction safety outranks leg-lengthening).
- **Heels** — block heel pump + the Statement Mule (both Phase 3 statement, 2.5–3", rare-occasion, two different silhouettes not a duplicate); [`anchor-heel/`](anchor-heel/) "Anchor One" (Must-Have, 2.0–2.25", everyday) — the moderate-heel-worn-often piece this category's own README argued was the better investment, built out with its own full vision doc and manufacturing brief given how deep the spec runs (3 variations, dedicated tech pack).
- **Sandals** — the Barely There Sandal (Phase 2, two versions: Everyday Strap and Dressy Slide, hybrid leather/fabric straps for durability without losing the delicate look) — romantic dry-weather open shoe.
- **Recovery** — the Yoga/Recovery Shoe, the one shoe category with no competing design priority against maximum comfort.
- **Jelly (Soft Structure)** — [`shoes/jelly/`](shoes/jelly/) Experimental seasonal sub-line (5 silhouettes, shared molded footbed + silver chain-link hardware). Fills warm-weather water / wipeable / translucent-color gap the leather sandal and rain boot don't cover. Documented exception to “patina over polish”: replaceable TPU/PVC, not heirloom. Hero everyday jelly flat sources first; expand only after trial.

### Accessories (`/accessories/`)
**Built: 6 items.** This category carries the most direct Starlink One integration in the whole system:
- **Layering jewelry** — sterling silver layering necklace/bracelet set (Phase 1), a heart-emerald statement pendant (Phase 3 fine jewelry) — chain-link detailing and stone color are deliberate callbacks to the ring's own design. This is where the ring gets "matched," not competed with.
- **Hair** — ribbons and silk scrunchies (Phase 2) — a signature LoveShackFancy x Target detail category, pulling heavily from Blush Mauve/Lavender Mist/Periwinkle.
- **Belts** — chain-link belt (Phase 2) — the single most direct hardware echo of Starlink One available in the accessories category.
- **Bags** — everyday crossbody bag (Phase 1, neutral colorway) before any statement bag.
- **Scarves** — everyday silk scarf (Phase 2), styling flexibility (neck, bag, hair).

### Dresses (`/dresses/`)
**Added during Phase 3.** A dress replaces both a top and a bottom at once and doesn't belong filed under either — this category exists because the Phase 3 build plan called for "a statement romantic piece built specifically to showcase the ring," and that piece turned out to be a dress. **Built: 2 items** — the ring statement dress (opaque Emerald showcase) and the sheer overlay dress (Soft Light, opaque underlayer required). Stays intentionally small; this is occasion dressing, not everyday rotation.

## Full Looks (`/full-looks/`)
Not a garment category — this is the assembly layer. **Built: 7 looks**, spanning Phase 1 essentials through Phase 3 statement and Soft Light / Soft Structure Experimental looks, each documenting a complete outfit and checking it against the color system and the ring (Soft Light looks also check [`translucent-system.md`](translucent-system.md)).

## Soft Light (cross-category)
Not a garment folder root — doctrine lives in [`translucent-system.md`](translucent-system.md). Pieces are filed in their real categories (`tops/translucent/`, skirts, outerwear, dresses) and assembled in full-looks 04–06. Rhymes with Soft Structure jelly footwear; does not replace it.

## Cross-Category Rules

1. **Every item lives in exactly one category/subcategory folder** and follows the priority tiers in [`priority-system.md`](priority-system.md).
2. **Color choices default to the 9-color palette** in `color-system.md` unless the item is explicitly an Experimental/Phase 3 bet.
3. **Hardware is silver-family only**, system-wide — this is a hard rule, not a per-item judgment call, because it's what keeps every accessory compatible with Starlink One by default.
4. **Fit rules from the manifesto apply everywhere**, not just bottoms — rise/inseam gets the most explicit treatment because bottoms was built first, but sleeve length, hem length, and proportion-to-64" apply with equal rigor to tops, outerwear, and dresses when that category is built.
