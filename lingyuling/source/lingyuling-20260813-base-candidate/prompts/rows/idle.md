Create one horizontal animation strip for Codex pet `lingyuling`, state `idle`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 凌玉灵，年轻优雅的女性修仙者。脸部以参考图1至3为准：白皙鹅蛋脸，细长灰褐色眼睛，平直柔和眉形，小巧鼻唇，沉静温柔而略显清冷；深棕近黑长发，中分前发与两侧长鬓，后发半束，右侧佩戴小型银金色弧形梳状发饰。整体服装以参考图4为准：浅灰白交领长袍，宽袖，层叠垂坠裙摆，肩部深灰护片，腰间宽幅古金色结构腰封，前胸至腰部有细长金色装饰，裙身带克制的金色纹样。单人紧凑全身、约三头身、正面轻微三分之四站姿，双手和双脚完整可见，服装轮廓清楚，主体尽量占满192x208单元格安全区。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `3d-toy`: Stylized 3D toy mascot with smooth rounded forms, simple materials, clear silhouette, and no photoreal complexity. User style notes: 精致中国3D动漫Q版，约三头身；与仓库现有银月、宋玉、慕沛灵一致的面部精细度、柔和材质、正面柔光、色彩饱和度与清晰轮廓；不是幼儿卡通，不是写实成人比例。纯色抠图底，无场景、底座、文字、水印、投影或接触阴影。.
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
