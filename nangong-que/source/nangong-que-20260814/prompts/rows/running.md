Create one horizontal animation strip for Codex pet `nangong-que`, state `running`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 已批准B1形象方向。独立生成pet-safe生产基本图：严格正面、单人紧凑全身、约三头身，完整显示黑色高髻发簪、银白三瓣额纹、细长杏眼、珍珠坠饰、双手、深青黑银纹宽袖外袍、蓝紫交领内衫、束腰长裙与双脚；以192x208显示为目标，主体充分占据安全区并保持清晰脚底基线；背景固定完全均匀纯洋红#FF00FF，无场景、地面、阴影、底座、文字或特效。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 精致中国3D动漫Q版，系列风格对齐银月、宋玉、慕沛灵；脸部成熟清冷，避免娃娃圆眼；材质精细但小尺寸轮廓清楚。.
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Working loop: focused active-task processing, thinking, typing, scanning, or effortful concentration; not literal foot-running, jogging, sprinting, treadmill motion, raised knees, long steps, pumping arms, or directional travel.

State requirements:
- Show the pet actively working or processing, as if running a task: focused posture, busy hands or paws, purposeful bobbing, thinking motion, tool or prop motion only if already part of the pet identity, or other non-locomotion activity.
- Do not show literal foot-running, jogging, sprinting, treadmill motion, raised knees, long steps, pumping arms, directional travel, speed lines, dust clouds, floor shadows, motion trails, or detached motion effects.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
