Create one horizontal animation strip for Codex pet `yunheng`, state `waiting`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 中国古风仙侠年轻男性，明确男性气质，白色长发半束，月白与淡青层叠仙袍，银金和玉色细节点缀，宽袖衣摆与腰间飘带轻盈飘逸；清冷温润、克制出尘，精致国风插画质感，袖珍全身比例但不幼儿化、不女相；不用武器，不添加场景、文字、光环、阴影或漂浮特效。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `painterly`: Painterly mascot with simplified brush texture, readable forms, stable palette, and enough edge clarity for clean extraction. User style notes: 精致中国古风角色插画，清晰硬边与简化大形，适合192x208宠物单元格；保持全身轮廓、男性面容与白发白衣细节在小尺寸可读。.
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Needs-input loop: expectant asking pose for approval, help, or user input.

State requirements:
- Show that Codex needs approval, help, or user input through an expectant asking pose.
- Keep the motion patient and readable, without turning it into ordinary idle or review.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
