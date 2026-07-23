Create one horizontal animation strip for Codex pet `songyu`, state `running-right`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 8 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 8 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 宋玉，约三头身精致中国3D动漫Q版成年女修；深棕黑长发、灰蓝眼睛、白玉云纹冠与两侧羽翼玉饰、双层红绳项链、青白渐变衣裙与深青叠绕腰封。jumping必须表现双手捧青绿色小茶杯嘟嘴吹茶，不做跳跃且无蒸汽；running-right与running-left必须表现人物清晰可见的侧身御空飞行、胸前法诀、长发袖裙向后飘动，完全无光球、遁光外壳、尾迹或速度线。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 与仓库 yinyue 宠物同系列：精致中国3D动漫Q版、约三头身、柔和材质、干净轮廓、成年温柔清冷气质、小尺寸可读。.
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Continuous rightward cultivator flight loop with Song Yu clearly visible and no escape-light sphere or energy shell.

State requirements:
- Show Song Yu in a compact three-quarter side view flying toward screen-right, with her body inclined forward about 15 degrees and her face and gaze unmistakably directed right.
- Keep one hand near the chest forming a restrained cultivation hand seal; let the other arm and wide sleeve stream naturally backward.
- Her long dark hair, translucent sleeves, ribbons, and skirt layers flow toward screen-left behind her in a coherent alternating wave across all 8 frames.
- Keep the complete character visible. Do not surround, cover, or backlight her with any orb, light ball, escape-light shell, aura, glow, tail, streak, or energy effect.
- Use subtle vertical bobbing plus alternating hair and fabric follow-through to create a seamless continuous flight cycle; do not repeat takeoff or landing within the loop.
- The row must unmistakably face and travel right.
- The movement cadence must alternate visibly across the 8 frames instead of repeating one nearly static stride.
- Do not draw speed lines, dust clouds, floor shadows, motion trails, or detached motion effects.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
