Create one horizontal animation strip for Codex pet `nangong-que`, state `idle`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 已批准B1形象方向。独立生成pet-safe生产基本图：严格正面、单人紧凑全身、约三头身，完整显示黑色高髻发簪、银白三瓣额纹、细长杏眼、珍珠坠饰、双手、深青黑银纹宽袖外袍、蓝紫交领内衫、束腰长裙与双脚；以192x208显示为目标，主体充分占据安全区并保持清晰脚底基线；背景固定完全均匀纯洋红#FF00FF，无场景、地面、阴影、底座、文字或特效。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 精致中国3D动漫Q版，系列风格对齐银月、宋玉、慕沛灵；脸部成熟清冷，避免娃娃圆眼；材质精细但小尺寸轮廓清楚。.
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Calm low-distraction resting loop: subtle breathing, tiny blink, slight head/body bob, and only quiet persona-preserving motion.

State requirements:
- CRITICAL: idle is the low-distraction baseline state and the first frame is also used as the reduced-motion static pet.
- Use only subtle idle motion: gentle breathing, a tiny blink, a slight head or body bob, a very small material sway, or another quiet motion that fits the pet persona.
- Keep the pet essentially in the same pose, facing direction, silhouette, markings, palette, and prop state across all 6 frames.
- Idle variation must stay calm but still read as animation; do not repeat effectively identical copies across the loop.
- Do not show waving, walking, running, jumping, talking, working, reviewing, emotional reactions, large gestures, item interactions, or new props.
- Feet, base, body, or object anchor should remain planted or nearly planted.
- The first and last frames should be very close visually so the loop feels calm and does not pop.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
