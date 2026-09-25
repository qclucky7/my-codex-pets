Create one horizontal animation strip for Codex pet `liyingning`, state `idle`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 候选A为唯一权威形象参考。精致中国3D动漫Q版，约三头身；黑发齐刘海、两侧环髻、双前辫、暖棕杏眼；左侧灰白纹样宽袖、右侧深青护肩护臂、酒红斜胸甲银边、黑色腰甲、赭黄色垂带、深青下裙、黑银短靴。右手稳定握住腰侧带鞘长剑；暖阳宝玉为腰间深色系绳悬挂的浅暖白色扁长水滴玉坠，带淡金雕纹，必须清晰可辨。idle为持剑待机；jumping不跳跃，改为双脚着地、低头并用空着的左手轻触暖阳宝玉再复位的五帧动作。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 与仓库现有银月、宋玉、慕沛灵一致的精致中国3D动漫Q版材质、光照、饱和度和清晰轮廓。生产基本图须正面、紧凑全身、充分占据192x208单元格安全区域。.
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
