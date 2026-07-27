Create one horizontal animation strip for Codex pet `meining`, state `failed`.

Use the attached canonical base for identity. Use the attached layout guide only for slot count, spacing, centering, and padding; do not draw the guide.

Output exactly 8 full-body frames in one left-to-right row on flat pure user-selected #FF00FF. Treat the row as 8 invisible equal-width slots: one centered complete pose per slot, evenly spaced, with no overlap, clipping, empty slots, labels, or borders.

Identity: same pet in every frame: 锁定用户确认的融合形象：左款发型发饰服装与端庄站姿，中款温柔灵秀脸。概念展示图只作身份参考，必须重新生成 pet-safe 生产基本图。生产基本图为单人紧凑全身、约三头身成年气质，主体充分占据 192x208 单元格安全区，纯洋红背景，无渐变和阴影。蓝灰瞳，黑色中分双侧低髻与长发，金铜叶片发饰、青绿宝石、垂珠耳坠，青白交领长裙、深青腰封、古铜腰饰、白色花枝刺绣。idle 仅呼吸眨眼与极轻发梢袖摆变化；jumping 不跳跃，改为温柔托脸动作；running-right 和 running-left 必须与 idle 保持相同视觉身高、头部大小、整体尺度和脚底基线。. Preserve silhouette, face, proportions, markings, palette, material, style, and props.
Style: Pet-safe sprite: compact full-body mascot, readable in a 192x208 cell, clear silhouette, simple face, stable palette/materials, and crisp edges for chroma-key extraction. Style `auto`: Infer the most appropriate pet-safe style from the user request and reference images, then keep that exact style consistent across every row. User style notes: 与仓库银月、宋玉、慕沛灵一致的精致中国3D动漫Q版风格；紧凑约三头身，大头小身但保持成年女性五官；服装纹样适度简化，宽袖与长裙不得造成主体缩小；清晰轮廓，细腻丝绸与发丝材质，小尺寸身份辨识度优先。.
Animation continuity: keep apparent pet scale and baseline stable within the row unless the state itself intentionally changes vertical position, such as `jumping`. Move the pose within the slot instead of redrawing the pet larger or smaller frame to frame.

State action: Blocked/failed loop: slumped or deflated reaction with sad or closed eyes.

State requirements:
- Show failure through slumped pose, drooping ears/limbs, closed or sad eyes, and lower body position.
- Tears, small smoke puffs, or tiny stars are allowed only if attached to or overlapping the pet silhouette and kept inside the same frame slot.
- Do not draw red X marks, floating symbols, detached stars, separated smoke clouds, falling tear drops, dust, or other loose effects.

Clean extraction: crisp opaque edges, safe padding, no scenery, text, guide marks, checkerboard, shadows, glows, motion blur, speed lines, dust, detached effects, stray pixels, or chroma-key colors inside the pet.
