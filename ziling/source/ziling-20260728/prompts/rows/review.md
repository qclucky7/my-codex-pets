Create one horizontal animation strip for Codex pet `ziling`, state `review`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 《凡人修仙传》动漫角色紫灵。脸部身份以参考图1-3为准：白皙精致的鹅蛋脸、紫色瞳眸、黑色长发与紫色半透明面纱。服装以参考图4的紫蓝色全身裙装、金色腰饰与发饰为准。基础姿态取参考图5双手在腰腹前自然交叠的含蓄仪态，但必须改成身体、脸和视线都正面对镜头。单人紧凑全身，完整双手和双脚，约三头身。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 精致中国3D动漫Q版，约三头身，面部精细但轮廓适合192x208桌宠小尺寸；材质、饱和度、柔和正面棚拍光和系列现有银月、宋玉、慕沛灵一致。纯洋红背景，无场景、底座、阴影、文字、水印或特效。.
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Ready-review loop: focused inspection of completed output with lean, blink, narrowed eyes, head tilt, or paw pose.

State requirements:
- Show review through lean, blink, narrowed eyes, head tilt, or paw/hand position.
- Do not add magnifying glasses, papers, code, UI, punctuation, symbols, or other new props unless they already exist in the base pet identity.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
