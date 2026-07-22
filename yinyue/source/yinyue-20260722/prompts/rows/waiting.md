Create one horizontal animation strip for Codex pet `yinyue`, state `waiting`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 6 full-body frames in one left-to-right row on flat pure magenta #FF00FF. Treat the row as 6 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 凡人修仙传动漫银月的人形造型。娇小灵动的银发狐耳少女，长银白发，银白狐耳带简化金属耳环，一蓝一琥珀异色瞳；月白银纹短裙、红色束腰，白色绒毛领与袖口，白色长靴。气质俏皮可爱又带灵狐机敏，比例为适合桌面 pet 的 Q 版人形全身，不携带武器。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 高品质中国3D动漫风格的Q版角色，约3头身，清晰整洁的硬边造型，服饰细节简化但有质感，适合缩小到192x208像素；保持银发、狐耳、异色瞳、红腰带为固定辨识点。.
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Needs-input loop: expectant asking pose for approval, help, or user input.

State requirements:
- Show that Codex needs approval, help, or user input through an expectant asking pose.
- Keep the motion patient and readable, without turning it into ordinary idle or review.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
