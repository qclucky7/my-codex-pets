Create one horizontal animation strip for Codex pet `ziling`, state `jumping`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 5 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 5 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 《凡人修仙传》动漫角色紫灵。脸部身份以参考图1-3为准：白皙精致的鹅蛋脸、紫色瞳眸、黑色长发与紫色半透明面纱。服装以参考图4的紫蓝色全身裙装、金色腰饰与发饰为准。基础姿态取参考图5双手在腰腹前自然交叠的含蓄仪态，但必须改成身体、脸和视线都正面对镜头。单人紧凑全身，完整双手和双脚，约三头身。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 精致中国3D动漫Q版，约三头身，面部精细但轮廓适合192x208桌宠小尺寸；材质、饱和度、柔和正面棚拍光和系列现有银月、宋玉、慕沛灵一致。纯洋红背景，无场景、底座、阴影、文字、水印或特效。.
Animation continuity: keep apparent pet scale, full-body height, and both-feet baseline stable throughout the row. She never leaves the ground.

State action: `敛袖轻礼`, an elegant restrained greeting loop replacing literal jumping. This is a continuity repair: the previous middle pose dropped the head and enlarged the silhouette too abruptly. Frame 1 stands front-facing with both hands overlapped at the waist. Frame 2 gently draws both sleeves inward while the chin lowers only a tiny amount. Frame 3 reaches the shallowest point of a micro-bow, with the torso tilted forward no more than 6 degrees and the chin only slightly lower than frame 2. Frame 4 rises partway as the sleeves relax and the eyes return fully forward. Frame 5 returns gracefully to the original upright hands-overlapped pose.

State requirements:
- Keep the body, face, and gaze front-facing throughout.
- Both feet remain planted on the same baseline in all five frames; no jumping, hovering, bouncing, or vertical travel.
- Make the gesture read mainly through the hands and sleeves; the head motion is secondary and extremely subtle.
- Distribute the micro-nod evenly across frames 2, 3, and 4. No single-frame head drop, deep bow, closed-eye snap, or sudden silhouette expansion.
- Keep the eyes softly open in every frame. Maximum chin travel is about 5% of the head height and the torso tilt stays under 6 degrees.
- Adjacent poses must feel like consecutive moments: keep occupied area and outer silhouette within roughly 5% from frame to frame.
- Use subtle veil, sleeve, and skirt follow-through only.
- Preserve the same apparent body size and head size in every frame.
- Do not draw ground shadows, contact shadows, drop shadows, oval shadows, landing marks, dust, smears, bounce pads, motion marks, magic, or detached effects.
- Keep the background outside the pet perfectly flat chroma key with no darker key-colored patches.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
