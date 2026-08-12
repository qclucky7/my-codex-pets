Create one horizontal animation strip for Codex pet `hanli`, state `running-right`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 8 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 8 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 候选C已获用户批准但仅作设计依据。必须单独生成生产基本图：韩立严格正面站立、双眼直视、窄长灰褐眼、眉眼冷静克制、年轻俊朗且有男性英气，不能幼态或通用萌系大眼；半束长黑发和横向发簪；墨绿宽袖长外袍、浅灰蓝交领内衫、深色腰封、双手双脚完整。约三头身，按192x208单元格充分占位。jumping行不跳跃，改为青竹小轩时期左手托旧绢书研读、翻页、右手并指推演、颔首回看书页的五帧循环。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 精致中国3D动漫Q版，与银月、宋玉、慕沛灵系列统一；轮廓清晰、材质细腻、正面眼神在小尺寸仍可辨识。.
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Dragging-right loop: show directional movement to the right through body and limb poses only.

State requirements:
- Show directional drag movement to the right through body, limb, and prop movement only.
- The row must unmistakably face and travel right.
- The movement cadence must alternate visibly across the 8 frames instead of repeating one nearly static stride.
- Do not draw speed lines, dust clouds, floor shadows, motion trails, or detached motion effects.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
