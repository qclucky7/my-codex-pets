Create one horizontal animation strip for Codex pet `mupeiling`, state `waiting`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 慕沛灵，约三头身精致中国3D动漫Q版成年女修。身份与脸部严格参考用户图：柔和鹅蛋脸、灰蓝大眼、纤细眉形、秀挺小鼻、自然珊瑚色嘴唇；深棕黑长发盘成高髻，额前中分碎发与两侧长鬓发，后发柔顺垂落；佩戴细长银珠流苏耳饰。服装必须采用参考图2至4的橙红色版本：橙红交领/深V内层长裙、暖橙织纹与低调金边、米杏色半透明宽袖、收束高腰腰封；绝不使用绿色或青绿色衣装。气质温柔、清冷、略带忧郁，保持成年女性而非幼童。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 与仓库 songyu、yinyue 的宠物同系列：精致中国3D动漫Q版、约三头身、大头小身但保持成年女性五官、柔和材质、干净轮廓、全身正面站姿、小尺寸可读；脸部相似度优先，服装橙红色优先。.
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Needs-input loop: expectant asking pose for approval, help, or user input.

State requirements:
- Show that Codex needs approval, help, or user input through an expectant asking pose.
- Keep the motion patient and readable, without turning it into ordinary idle or review.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
