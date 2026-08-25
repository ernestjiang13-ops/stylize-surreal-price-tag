# Style Profile: Warped Surreal Price-Tag Airbrush

## Contents

- Core visual DNA
- Structural grammar
- Distortion scale
- Canvas and composition grammar
- Automatic surreal-element pool
- Accessory attachment grammar
- Rendering grammar
- Price-tag grammar
- Reference routing
- Failure modes

## Core visual DNA

The reference family depicts ordinary retail objects, foods, tools, and creatures as strange collectible commodities. Each image isolates a single recognizable subject on white, deforms it into an unstable sculptural silhouette, adds one or two impossible features, then marks it with a small price label. The result sits between low-fi airbrush illustration, early digital graphics, surreal product photography, and Y2K retail imagery.

The desired tension is recognizable versus strange: the viewer must identify the source subject immediately, then notice the restrained perimeter swelling, unexpected accessory, color, and retail labeling.

## Structural grammar

- Use one dominant subject and generous white negative space.
- Retain the complete base silhouette and two to four signature anchors.
- Keep the central axis, orientation, and internal feature placement stable.
- Deform only the perimeter through a few broad, low-amplitude, softly rounded outward swells that blend smoothly into the source outline.
- Prefer asymmetry and slightly awkward proportions.
- Add one logically attached accessory by default, not a collage of arbitrary decorations.
- Preserve the object's anatomy. Do not introduce holes, sockets, tunnels, ropes, tubes, or protruding masses without an explicit request.
- Keep the price element small and subordinate.

## Distortion scale

- Level 1: at least 98% silhouette retention; one or two barely visible broad outward rises, up to about 2% of subject width.
- Level 2: at least 95% silhouette retention; two or three gentle broad outward rises, up to about 4% of subject width. Default.
- Level 3: at least 90% silhouette retention; two to four visible but smooth outward swells, up to about 7% of subject width.
- Level 4: at least 85% silhouette retention; two to four larger broad swells, up to about 10% of subject width, with the central axis stable.
- Level 5: at least 75% silhouette retention; two to five bold continuous perimeter swells, up to about 15% of subject width, without whole-form bending.

Use low-frequency outward contour changes. Each swell should span a long section of the perimeter, rise gently to a rounded crest, then ease back into the source outline. Space swells irregularly and vary their size so they feel organic, not sinusoidal. A distorted lemon remains one continuous, upright lemon shape; it does not become S-shaped, serpentine, pinched, regularly wavy, footed, lobed, dripping, perforated, or covered in small bumps.

## Canvas and composition grammar

- Ask only for output ratio and distortion level before every generation unless both were already provided. Choose the surreal element automatically.
- Default to portrait 3:4, interpreted as width:height = 3:4.
- Offer square 1:1, landscape 4:3, landscape 16:9, portrait 9:16, follow source, and a free-form custom ratio or exact pixel size.
- For portrait 3:4, keep the complete subject at roughly 60–75% of canvas height, centered with balanced white margins.
- Adapt subject scale to other ratios while preserving the complete silhouette and all accessories.
- Never satisfy a ratio by cropping the subject, cutting off an accessory, or allowing the form to touch the frame.

## Automatic surreal-element pool

Build a subject-appropriate eligible set privately and randomly choose exactly one element. Do not show a choice menu or ask the user to select. Track elements already generated in the visible conversation and sample without replacement: remove all used elements before drawing. Do not repeat until every suitable element for the subject category has been used. When the pool is exhausted, start a new cycle while still excluding the immediately previous element.

### Wearable and clipped

- Sunglasses across an implied face or broad upper plane.
- Headphones wrapping around two opposing sides.
- Bow hair clip, flower hairpin, or barrette clipped to a stem, leaf, top edge, hair, or fabric fold.
- Tiny beret, cap, or soft crown resting on a stable top plane.
- Brooch attached to fabric, a soft surface, or a broad front plane.

### Small living visitors

- Caterpillar crawling along a peel, leaf, rim, handle, or long surface.
- Snail resting on a broad stable surface with visible contact.
- Ladybug or beetle landed on a leaf, edge, or front plane.
- Butterfly or moth perched on an upper edge, stem, leaf, shoulder, or handle.
- Tiny frog resting on a stable top or side plane.
- Small gecko gripping a broad side surface.

### Growing and falling

- One or two tender sprouts emerging from an existing seam, stem, top opening, or natural crease without creating a hole.
- A small moss patch following an existing surface contour.
- A tiny mushroom cluster growing only from an existing seam, crease, soil-like area, or broad organic surface.
- Falling leaves originating from an existing stem or leaf cluster.
- Loose petals drifting from an existing flower, bud, or floral attachment.
- A tiny flower cluster growing from an existing stem, seam, or top opening.

### Surface attachments

- A fabric patch or crooked bandage adhered to a broad surface.
- A zipper following an existing seam, fold, or long flat surface without opening a cavity.
- A safety pin, binder clip, or clothes peg gripping a real thin edge, leaf, fold, or flap.
- A small button or brooch attached to fabric or a naturally broad front plane.

Never use rings, hoops, bracelets, circular bands, necklaces, chains, or loop-like jewelry. Simple circular loops are visually ambiguous and can read as unexplained objects. Exclude any element that requires drilling a hole, inventing a limb, or adding a rope or tube.

Route by subject:

- Produce and plants: prioritize caterpillar, snail, ladybug, butterfly, sprout, moss, falling leaf, petals, or flower clip.
- Food and tableware: prioritize sunglasses, caterpillar, ladybug, tiny frog, bandage patch, clip, or a small top-resting hat when physically plausible.
- Tools, appliances, and electronics: prioritize headphones, sunglasses, barrette, zipper along a seam, binder clip, gecko, or butterfly.
- Soft goods and clothing: prioritize brooch, hair clip, zipper, patch, butterfly, beetle, moss, or mushroom cluster.
- People and animals: prioritize sunglasses, headphones, hair clip, beret, butterfly, ladybug, falling petals, or a small resting creature that does not obscure the face.

## Accessory attachment grammar

Use accessories with an obvious support point and purpose:

- Sunglasses sit across the implied face or upper front plane.
- Headphones wrap around two sides with a connected headband.
- Hair ornaments clip to a leaf, stem, top edge, or hair-like detail.
- Caterpillars crawl on a surface or leaf and visibly touch it.
- Falling leaves originate from a visible stem or leaf cluster and fall beside or below it.

Use exactly one automatically drawn unused element. Maintain believable scale, perspective, overlap, and contact. Never cut a new hole to attach an accessory. If the drawn element has no plausible attachment point, discard it before generation and draw another unused eligible element.

## Rendering grammar

- Build volume from blurred spray gradients rather than clean geometric shading.
- Use visible fine grain, especially in black shadow transitions and around edges.
- Combine saturated acidic colors with dense black shading.
- Add small hard or soft white highlights to suggest shiny, synthetic surfaces.
- Let color wander across form independently of real material color.
- Keep edges slightly fuzzy or uneven while maintaining a readable silhouette.
- Avoid polished photorealistic CGI, clean vector gradients, uniform clay materials, and smooth studio shadows.

## Price-tag grammar

Build a viable on-subject candidate set and randomly choose one position per generation unless the user specifies the location. Do not repeatedly default to the center or lower-right. Exclude positions that cover recognition anchors, faces, surreal elements, or important textures. Candidate positions include:

- Upper-left or upper-right surface.
- Mid-left or mid-right surface near the outer edge.
- Lower-left or lower-right surface.

The center of the tag must remain inside the subject silhouette. Most of the label must sit directly on the visible surface; a small part may overlap the outer contour only when the rest stays visibly attached. Show contact through curvature, overlap, slight occlusion, or subtle contact shadow. Never leave a white gap between tag and subject.

Then choose one tag form:

- Oval retail sticker attached to the object's body.
- Small rectangular sticker placed at an angle.
- Jagged burst label for louder commercial energy.
- Torn ticket shape for a handmade low-fi feeling.

Never use a floating, separate, suspended, or dangling tag. Never tie it to a handle, stem, string, rope, or appendage.

Use a high-contrast tag color drawn from the palette. Always use `$`. Paint the symbol and every numeral directly as distorted handmade spray lettering rather than applying a font: vary each glyph's lean, height, width, curvature, spacing, and stroke thickness; use an irregular baseline, fuzzy overspray, feathered pigment, soft color bleed, broken coverage, and visibly hand-made imperfections. A clean font placed on a sprayed label is a failure. Keep the amount legible, but never use upright uniform glyphs, crisp vector edges, or mechanical alignment. The amount is decorative rather than a factual claim unless the user supplies an exact price.

## Reference routing

Select references by structural similarity and effect, not by subject alone.

| Reference | Best use |
|---|---|
| `ref-kettle.jpg` | Containers, appliances, handles, bulbous volume, sticker on body |
| `ref-bag.jpg` | Fabric, clothing, soft goods, sagging and draped deformation |
| `ref-stack.jpg` | Food, stacked products, framing and airbrush rendering; do not copy its voids at levels 1–2 |
| `ref-headphones.jpg` | Electronics, portraits, rounded modular additions |
| `ref-tomato.jpg` | Produce, organic matter, inflated glossy body, ticket label |
| `ref-pepper-creature.jpg` | Produce, color and airbrush rendering; do not copy its creature appendages unless explicitly requested |
| `ref-lobster.jpg` | Animals, segmented forms, biomorphic exaggeration, label rendering only; do not copy floating placement |
| `ref-ribbed-pepper.jpg` | Produce, strong inflation, simplified silhouette, sticker integration |
| `ref-scissors.jpg` | Tools and preserved functional anchors; do not copy the dangling tag placement |
| `ref-cups.jpg` | Tableware, stacking, melting, tonal restraint, small label |
| `ref-stars.jpg` | Secondary surreal motifs, simple spiked forms; do not use as the main object reference |

Use two to four references total. Favor one structural reference, one rendering reference, and optionally one price-tag reference.

## Failure modes

- Merely applying rainbow color while preserving the source unchanged.
- Replacing the source subject with an object from the references.
- Distorting a lemon or other simple fruit into a footed, lobed, dripping, or perforated object.
- Bending the whole subject into an S, snake, wave, or side-to-side zigzag.
- Creating a repeated, regular ripple around the perimeter instead of a few irregular broad rises.
- Using inward pinches, deep dents, sharp spikes, or isolated tumor-like bumps.
- Using clusters of small bumps as a substitute for a few broad perimeter swells.
- Adding a hole with a rope, tube, loop, or unknown object passing through it.
- Adding accessories without a believable attachment point, scale, overlap, or contact.
- Using generic fantasy scenery, cosmic backgrounds, smoke, or neon city imagery.
- Producing clean plastic 3D rendering without airbrush grain.
- Adding large promotional typography or multiple price stickers.
- Cropping the main subject or allowing its extremities to touch the frame.
- Asking the user to choose a surreal element instead of selecting one automatically.
- Using rings, hoops, bracelets, circular bands, chains, or other ambiguous loop jewelry.
- Repeating any surreal element before the suitable pool completes its no-repeat cycle.
- Ignoring the selected ratio or defaulting to square when portrait 3:4 was selected.
- Making the price tag the focal point.
- Reusing the same default tag position instead of randomly choosing from viable zones.
- Placing the tag over a recognition anchor, face, accessory, important texture, or against the frame edge.
- Floating, suspending, or dangling the price tag outside the subject, or leaving a white gap between tag and object.
- Using `¥` or another currency symbol instead of `$`.
- Rendering the price as crisp digital typography instead of crooked airbrushed handwriting.
- Keeping the glyphs uniform while adding spray texture only to the tag background.
- Copying one reference composition too literally instead of transferring the shared style system.
