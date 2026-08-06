Create one horizontal animation strip for Codex pet `ziling`, state `idle`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 《凡人修仙传》动漫角色紫灵。脸部身份以参考图1-3为准：白皙精致的鹅蛋脸、紫色瞳眸、黑色长发与紫色半透明面纱。服装以参考图4的紫蓝色全身裙装、金色腰饰与发饰为准。基础姿态取参考图5双手在腰腹前自然交叠的含蓄仪态，但必须改成身体、脸和视线都正面对镜头。单人紧凑全身，完整双手和双脚，约三头身。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 精致中国3D动漫Q版，约三头身，面部精细但轮廓适合192x208桌宠小尺寸；材质、饱和度、柔和正面棚拍光和系列现有银月、宋玉、慕沛灵一致。纯洋红背景，无场景、底座、阴影、文字、水印或特效。.
Animation continuity: use the attached approved `jumping` strip as the exact visual scale and silhouette-width reference. Match its slimmer body, narrower hair/shoulder/skirt outline, head size, full-body height, and both-feet baseline in every idle frame. At final 192x208 size, aim for the same roughly 64-68 pixel-wide occupied silhouette as `jumping`, not the old wider or chubbier idle proportions. Move only facial eyelids and tiny breathing details; never redraw the pet larger, wider, shorter, or rounder frame to frame.

State action: Calm low-distraction resting loop: the head, face direction, hair silhouette, shoulders, torso, hands, and feet stay spatially locked; motion comes only from a tiny chest/sleeve breathing change and one slow blink.

State requirements:
- CRITICAL: idle is the low-distraction baseline state and the first frame is also used as the reduced-motion static pet.
- Six-frame sequence: neutral open eyes; tiny inhale with hands still overlapped; eyelids half lower; one soft blink; eyelids reopen; return nearly exactly to frame 1.
- CRITICAL: no head shake, head turn, nod, tilt, bob, chin movement, gaze drift, shoulder sway, torso lean, or lateral hair movement. Keep the face and purple eyes aimed straight at the viewer whenever the eyes are open.
- Use only subtle breathing visible in the upper sleeves/chest by a few pixels and the slow blink. Keep the waist, skirt, hair outline, hands, and feet fixed.
- Match the approved `jumping` strip's slim silhouette. Do not make the cheeks, head, shoulders, upper arms, waist, skirt, or hair mass wider or rounder.
- Keep the pet essentially in the same pose, facing direction, silhouette, markings, palette, and prop state across all 6 frames.
- Idle variation must stay calm but still read as animation; do not repeat effectively identical copies across the loop.
- Do not show waving, walking, running, jumping, talking, working, reviewing, emotional reactions, large gestures, item interactions, or new props.
- Feet, base, body, or object anchor should remain planted or nearly planted.
- The first and last frames should be very close visually so the loop feels calm and does not pop.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
