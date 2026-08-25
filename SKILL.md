---
name: stylize-surreal-price-tag
description: Transform an uploaded photo by isolating its main subject, preserving its silhouette and stable central axis, applying a user-selectable 1–5 level of gentle broad outward contour swelling, automatically choosing one plausible nonrepeating surreal element, and adding an airbrushed handwritten dollar price tag pasted directly onto the subject. Before generating, ask only for distortion level and aspect ratio; default to level 2 and portrait 3:4. Randomly select surreal elements without replacement within the visible conversation, and never use rings, hoops, or ambiguous circular loops. Use when the user asks to extract and surrealize a photo subject, add natural rounded contour rises, or match the bundled warped-price-tag style. Works with products, objects, food, animals, and people. Do not use for ordinary retouching or cleanup; do not create an overall S-curve, unexplained hole, rope, tube, appendage, or cluster of small bumps, and never float or dangle the price tag outside the subject.
---

# Stylize Surreal Price Tag

Turn a photo's main subject into an immediately recognizable surreal retail artifact. Preserve the base form, central axis, and orientation first, then add restrained outward contour swelling, logically attached accessories, and a handmade price label. Analyze the image and create the edited image instead of returning only a prompt.

## Required reference

Read [references/style-profile.md](references/style-profile.md) before the first generation in a conversation. Select two to four relevant images from `assets/references/` as style references; do not use all references indiscriminately.

## Workflow

### 1. Inspect the source

- View the source image before editing when it has not already been inspected.
- Identify the dominant subject by visual salience, scale, focus, and semantic importance.
- Record two to four recognition anchors that must survive, such as silhouette, handle, stem, face, opening, limbs, or signature proportions.
- Separate the dominant subject from the original background. Exclude incidental people, props, text, shadows, scenery, and reflections unless they define the subject.
- If several subjects compete equally, ask the user which subject to transform. Otherwise proceed without reconfirmation.

### 2. Confirm distortion and canvas before generating

- Before calling any image-generation or image-editing tool, ask the user to confirm the distortion level and output ratio together in one compact question.
- Do not ask the user to choose the surreal element. Select it automatically after the source is inspected.
- Do not generate until both user choices are known. If the user already provided one choice, ask only for the missing choice. If both are explicit, proceed without asking again.
- If the user replies “默认”, “按默认”, or an equivalent phrase, use distortion level 2 and portrait 3:4, then automatically choose the surreal element.
- Use this question format:

  > 出图前请确认两个选项：
  >
  > 1. 扭曲程度：1–5级（默认2级）
  >
  > 2. 画面比例：竖版3:4（默认）／方形1:1／横版4:3／横版16:9／竖版9:16／跟随原图／自定义比例或像素

- Accept a custom ratio such as `2:3`, `4:5`, or `5:7`, or exact dimensions such as `1500×2000 px`.
- Treat “竖版3:4” as width:height = 3:4. Keep the full subject centered with generous white space and no cropping.

### 3. Make the art direction decision

Choose the following automatically from the subject's structure:

- The confirmed distortion level from 1–5.
- Two or three broad, softly rounded outward contour rises placed asymmetrically along the perimeter. Keep the rises low-amplitude, long, and smoothly blended into the original outline.
- One automatically and randomly selected surreal element that is plausible for the source and unused in the current no-repeat cycle.
- A three-to-five-color acidic palette with deep black shading and small white highlights.
- A price-tag shape, randomly selected viable placement, irregular angle, color, and fictitious decorative dollar amount.

Use this distortion scale:

| Level | Shape treatment |
|---|---|
| 1 | Preserve at least 98% of the silhouette; add one or two barely visible, broad outward rises, each no more than about 2% of subject width. |
| 2 | Preserve at least 95% of the silhouette; add two or three gentle, broad outward rises, normally no more than about 4% of subject width. Default. |
| 3 | Preserve at least 90% of the silhouette; add two to four clearly visible but smooth outward swells, normally no more than about 7% of subject width. |
| 4 | Preserve at least 85% of the silhouette; enlarge two to four broad perimeter swells, normally no more than about 10% of subject width, while preserving the stable central axis. |
| 5 | Preserve at least 75% of the silhouette; use two to five bold but continuous perimeter swells, normally no more than about 15% of subject width, without bending the subject into an S or wave. |

Treat these percentages as art-direction guides rather than measurements that justify cropping or shape loss. At every level, keep the subject's central axis, top-to-bottom orientation, and main mass stable. Vary only the outer perimeter with broad convex swells. Do not use an overall S-curve, serpentine bend, sinusoidal wave, repeated alternating concave-convex rhythm, waist-like pinch, or inward notch. Do not simulate distortion with small feet, toes, bubbles, drips, knots, spikes, or isolated tumor-like lumps.

### 4. Preserve recognizability while distorting

- Preserve the complete outer silhouette and at least two recognition anchors at levels 1–3.
- Make the subject identifiable immediately, before the viewer notices the surreal treatment.
- Lock the subject's central axis, overall orientation, and internal feature placement before changing the contour.
- Apply only low-frequency outward contour changes: each rise must occupy a broad stretch of the perimeter, have a softly rounded crest, and transition gradually back into the source outline.
- Keep the swells irregularly spaced and unequal in size so they feel organic rather than like a regular wave pattern.
- Prefer outward convexity. Avoid deep inward dents, pinches, narrow waists, and alternating in-out undulation.
- Keep fine structural details subordinate to the outer contour; do not invent missing anatomy to create visual interest.
- For fruit and vegetables, preserve the continuous fruit body, natural bottom tip, stem, and leaf relationship. Do not turn the lower edge into feet, toes, repeated drips, or separate lobes unless the source already has those features.
- Do not cut holes, portals, sockets, tunnels, or cavities into the subject unless the source contains them or the user explicitly requests them.
- Preserve essential identity cues for a person or animal. Do not introduce extra facial features unless explicitly requested.
- Keep the full transformed subject in frame with comfortable white space; do not crop important extremities.

### 5. Attach surreal elements logically

- Build an eligible set from the pool and routing rules in [references/style-profile.md](references/style-profile.md). Keep only elements with an obvious wearing, clipping, resting, gripping, growing, landing, or falling relationship to the source.
- Maintain a used-element set from images generated in the visible conversation. Remove every used element from the eligible set, then randomly choose one remaining element. This is sampling without replacement, not weighted repetition.
- Do not repeat an element until every suitable element for the current subject category has been used. When the eligible unused set is exhausted, begin a new cycle but still exclude the element used in the immediately previous image.
- Add exactly one surreal element. Do not ask the user to choose and do not disclose the internal candidate list before generation.
- Never use a ring, hoop, bracelet, circular band, necklace, chain, or ambiguous loop-like jewelry. A simple circular loop does not read clearly enough as an intentional object.
- Prefer familiar accessories, small living elements, plant growth, or surface attachments with an obvious physical relationship to the subject.
- Place sunglasses across an implied face or the upper front plane.
- Place headphones over or around two sides of the subject; make the headband and ear cups visibly connect.
- Clip a hair ornament to a stem, leaf, top edge, or hair-like feature.
- Let a caterpillar crawl on the peel, surface, stem, or leaf with visible contact and believable scale.
- Let falling leaves detach from an existing leaf or stem and appear beside or below the subject.
- Match scale, overlap, contact shadow, perspective, and material treatment so the added element appears intentionally worn, held, resting, growing, or falling.
- Do not add unexplained ropes, loose tubes, empty loops, random handles, floating geometry, or body openings.
- If the randomly drawn element has no convincing relationship after closer inspection, discard it before generation and randomly draw another unused eligible element. Do not ask the user unless no valid element exists.

### 6. Build the style

- Use a clean white background by default. Use transparent background only when requested and supported.
- Render soft airbrushed gradients, visible spray grain, fuzzy transitions, deep black edge shadows, colored halos, and sparse hard white highlights.
- Favor acidic yellow, orange-red, magenta, violet, cyan, turquoise, and green, balanced by black.
- Make the finish intentionally low-fi and hand-processed rather than polished vector art or conventional 3D rendering.
- Keep one dominant isolated subject. Avoid environmental scenes, ground planes, realistic cast shadows, borders, captions, logos, and unrelated typography.
- Compose for the confirmed aspect ratio. In the default portrait 3:4 canvas, keep the complete subject approximately 60–75% of the canvas height with balanced top, side, and bottom white space.

### 7. Add the price tag

- Include one small price tag as a required visual accent unless the user explicitly removes it.
- Randomize the price-tag position on the subject for every generation unless the user specifies a location. Do not repeatedly default to the center or lower-right.
- Form a viable set from the upper-left, upper-right, mid-left, mid-right, lower-left, and lower-right regions of the subject's visible surface. Exclude any candidate that covers a recognition anchor, face, surreal element, or important texture; then choose randomly from the remaining candidates.
- Paste the tag directly onto the subject's visible surface, or let a small portion overlap the outer contour while most of the tag remains physically attached to the subject. The tag center must fall inside the subject silhouette.
- Require visible physical contact through surface curvature, overlap, slight occlusion, or a subtle contact shadow. There must be no white gap between the tag and the subject.
- Never place the tag floating in background space, merely beside the subject, suspended outside it, or dangling from a string, rope, handle, stem, or appendage.
- Keep it secondary, normally about 4–8% of the subject's bounding box, and give it a slight irregular rotation rather than a mechanically straight alignment.
- Use an oval sticker, torn ticket, burst, or rectangular pasted label appropriate to the subject, but render the tag itself with irregular airbrushed edges rather than a crisp vector shape.
- Always use the `$` symbol. If the user supplies only a number, prefix it with `$`. Otherwise use a fictitious decorative value such as `$88.88` or `$99.99`.
- Paint the `$` and every numeral directly as distorted handmade spray lettering, never as a font or clean text overlay. Make individual glyphs lean in different directions, vary in height and width, bend or compress their shapes, sit on an irregular baseline, and use uneven stroke thickness.
- Add clear airbrush evidence to the lettering itself: fuzzy overspray, feathered pigment, soft dark edges, slight color bleed, broken coverage, and small hand-painted imperfections. Applying a spray texture behind an otherwise clean font does not satisfy this rule.
- Keep the amount readable. In the generation prompt, explicitly reject upright uniform glyphs, a straight baseline, consistent spacing, crisp vector edges, mechanical alignment, typeset appearance, and clean digital typography. After generation, do not edit or regenerate the image to correct the lettering.

### 8. Generate the edit

- Use the available image-editing or image-generation tool with the source photo and the selected bundled style references.
- Include the source photo first and no more than four selected style references when the tool has a reference limit.
- Describe the required preservation anchors, stable central axis, and unchanged orientation explicitly in the editing prompt.
- State the selected distortion level explicitly and translate it into the matching number and amplitude of broad outward contour rises.
- State the confirmed aspect ratio and orientation explicitly. Require the full subject to remain inside that canvas without cropping or touching the frame.
- Name the automatically selected surreal element and its exact attachment point. Describe how it touches, overlaps, clips to, rests on, grows from, lands on, or falls from the subject.
- State the randomly selected on-subject price-tag zone. Require the tag center to remain inside the subject silhouette, with most of the label pasted to the visible surface and no white gap. Describe the price characters as hand-painted image content rather than a font or text overlay.
- State that the style references control rendering language only; they must not replace the source subject with a kettle, bag, pepper, lobster, scissors, cup, or other reference object.
- Make exactly one image-generation or image-editing call for each user request and request a single final image, not variants.
- Do not request or present alternate versions, batches, grids, contact sheets, before-and-after pairs, or multiple compositions.
- If the tool nevertheless returns two or more candidates from the single call, compare them privately, select the one that best satisfies the skill, and expose only that one image. Do not expose, mention, or combine the other candidates.
- After the first generation completes, do not regenerate, edit, inpaint, retouch, upscale, or make any other modification call. Only perform a new generation or modification when the user explicitly requests it in a later message.

### 9. Check the result

Before delivering, verify:

- The source subject remains identifiable.
- The original background is removed.
- The output uses the confirmed aspect ratio; portrait 3:4 is used when the user selected the default.
- The selected 1–5 distortion level is respected and the outer silhouette remains recognizable.
- The subject's central axis and orientation remain stable; it does not bend into an S, snake, or wave.
- Distortion appears only as a few broad, natural, softly rounded outward contour rises, not a repeated ripple or cluster of small protrusions.
- No deep inward dent, narrow waist, sharp bump, spike, or tumor-like growth appears.
- No unexplained holes, tubes, ropes, loops, feet, toes, or drips appeared.
- Exactly one coherent surreal element is physically and semantically attached, resting, worn, growing, landed, or falling.
- The surreal element was randomly selected from the unused eligible pool, does not repeat within the active cycle, and is not a ring or ambiguous loop.
- One price tag is present and secondary.
- The price-tag position was randomly selected from viable on-subject zones and does not cover a recognition anchor, face, surreal element, or important texture.
- The tag is visibly pasted to the subject: its center is inside the silhouette, most of its area touches the surface, and no white gap separates it from the object.
- The tag is not floating, standing separately, or hanging outside the subject.
- The price uses `$`; every glyph is visibly distorted, individually irregular, hand-painted, and airbrushed rather than typeset.
- The lettering has an uneven baseline, inconsistent glyph size and lean, fuzzy overspray, soft bleeding edges, and nonuniform stroke coverage.
- Airbrush grain, acidic gradients, black edge shading, and white negative space match the reference family.
- The subject is complete and not accidentally cropped.
- No extra captions, logos, watermarks, scenery, or duplicated subjects appeared.

Use this check only to select the best candidate returned by the single generation call. Do not revise, regenerate, or modify the selected image automatically, even if a requirement is imperfect.

## Prompt scaffold

Adapt this scaffold to the source rather than copying it mechanically:

> Isolate the dominant subject from the uploaded photo and preserve [outer silhouette and recognition anchors]. Lock its central axis, top-to-bottom orientation, and internal feature placement; do not bend the whole subject. Compose on a [confirmed aspect ratio and orientation] canvas; keep the complete subject centered, fully inside the frame, and surrounded by generous white space. Apply distortion level [1–5] only along the outer perimeter: add [number] broad, low-amplitude, softly rounded outward contour rises, irregularly spaced and smoothly blended into the original outline. No overall S-curve, serpentine bend, regular wave, alternating inward-outward ripple, pinched waist, sharp local bump, feet, drips, holes, or unexplained openings. Add the automatically selected unused [surreal element] at [logical attachment point], visibly [worn/clipped/resting/growing/landed/falling] with believable contact and scale. Never use a ring, hoop, circular band, chain, or ambiguous loop. Render it with soft airbrushed spray grain, acidic [palette] gradients, deep black edge shadows, colored halos, and sparse white glossy highlights. Randomly select one viable price-tag zone on the subject's visible surface, excluding recognition anchors, the surreal element, and important textures. Paste one small irregular airbrushed [tag shape] there, reading `$[amount]`; keep its center inside the subject silhouette, most of its area touching the surface, and no white gap between label and object. Never float, suspend, or dangle the price tag outside the subject. Paint every character directly as distorted handmade spray lettering—not a font or text overlay—with differently leaning, stretched, compressed, unevenly sized glyphs, a crooked baseline, irregular spacing and stroke width, fuzzy overspray, feathered pigment, broken coverage, and soft color bleed. Keep it readable but never neat or typographic. Clean pure white background, isolated centered composition, complete subject, generous negative space. The reference images define only the visual language; do not copy their objects. Avoid photorealism, ordinary 3D, clean vector gradients, typeset price text, environmental scenery, extra text, and unrelated objects.

## Delivery

Return exactly one unmodified image from the single generation call and one short sentence naming the aspect ratio, distortion level, contour-rise treatment, automatically selected surreal element, and pasted price-tag treatment. Never display additional candidates or automatic revisions. Do not expose the full internal prompt unless the user asks for it.
