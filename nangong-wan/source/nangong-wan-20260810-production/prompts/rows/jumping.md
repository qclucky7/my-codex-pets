Create one horizontal animation strip for Codex pet `nangong-wan`, state `jumping`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 5 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 5 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 严格保留已批准基本图的圆润脸型、灰紫大眼、额心红纹、银蓝冠饰、黑色长发、冰蓝宽袖与深蓝长裙。约三头身，清冷端庄。jumping 行不跳跃、不腾空，改为正面站立掐诀：双手抬至胸前结印，短暂闭眼凝神，再轻微放松回到循环起点；双脚全程固定同一基线。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 精致中国3D动漫Q版，柔和瓷白皮肤，丝绸与薄纱材质，清晰轮廓，桌面小尺寸可读，系列风格与银月、宋玉、慕沛灵一致。.
Animation continuity: keep apparent pet scale, feet position, and baseline stable throughout all five frames. This customized `jumping` row never changes vertical position. Move only the hands, fingers, forearms, sleeves, eyelids, and subtle hair tips; never resize or lift the pet.

State action: A poised two-hand cultivation mudra with both feet planted. Frame 1 begins lifting both hands toward the chest. Frame 2 brings the fingertips together. Frame 3 holds a clear centered hand seal. Frame 4 maintains the seal with a brief focused eyelid lowering. Frame 5 relaxes the seal slightly toward the starting pose for a smooth loop.

State requirements:
- Do not jump, hover, lift, bounce, crouch, or leave the ground in any frame.
- Both shoes stay fully visible and fixed to exactly the same baseline and horizontal registration in all five frames.
- Both hands and fingertips must remain clearly readable at chest center, outside the wide sleeves.
- Keep elbows and sleeves close enough to the body that adjacent generated figures remain completely separated.
- Exactly one separate figure per slot; hair, fingers, sleeves, skirts, ornaments, and antialias fringes must never touch a neighboring pose.
- Do not draw ground shadows, contact shadows, drop shadows, oval shadows, landing marks, dust, smears, bounce pads, or motion marks under the pet.
- Keep the background outside the pet perfectly flat chroma key with no darker key-colored patches.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
