# 韩立·结丹巅峰

《凡人修仙传》动漫结丹巅峰时期韩立的 Codex Desktop Q 版动态桌宠。

形象采用精致中国 3D 动漫 Q 版造型，保留高束长发、银白前发、深蓝黑金纹法袍与双尖噬金虫金枪。`jumping` 状态不做跳跃，按已确认动作设计为双脚落地的摸枪流程：横枪、从枪头背面轻触检查，再回到初始姿势。

![韩立·结丹巅峰待机动画](assets/idle.gif)

## 动作总览

![韩立·结丹巅峰完整动作总览](assets/contact-sheet.png)

| 状态 | 效果 |
| --- | --- |
| `idle` | 沉静站立，双尖金枪斜背身后，呼吸与眨眼微动 |
| `running-right` | 无枪向右跑动，双臂自然交替摆动 |
| `running-left` | 无枪向左跑动，保持发型与衣饰侧别 |
| `waving` | 持枪抬手示意 |
| `jumping` | 双脚落地：横枪、从枪头背面轻触检查，再回到初始姿势 |
| `failed` | 克制地低头失落，再恢复站姿 |
| `waiting` | 竖枪等待确认，手臂与枪身无穿模 |
| `running` | 专注处理任务 |
| `review` | 凝神审阅结果 |
| Look directions | 16 个顺时针观察方向，金枪竖直背于身后 |

![韩立·结丹巅峰摸枪动画](assets/jumping.gif)

## 安装

在仓库根目录执行 PowerShell：

```powershell
$target = Join-Path $HOME ".codex\pets\hanli-jiedan-peak"
New-Item -ItemType Directory -Path $target -Force | Out-Null
Copy-Item .\hanli-jiedan-peak\pet.json, .\hanli-jiedan-peak\spritesheet.webp -Destination $target -Force
```

复制后重启 Codex Desktop，并在 pet 选择界面选择“韩立·结丹巅峰”。

## 图集规格与验证

| 项目 | 数值 |
| --- | --- |
| Sprite 版本 | 2 |
| 图集尺寸 | 1536 × 2288 |
| 网格 | 8 列 × 11 行 |
| 单帧尺寸 | 192 × 208 |
| 格式 | RGBA WebP |

最终图集已通过 v2 结构与透明背景校验、9 行动作检查、16 向语义检查、三份隔离方向盲测、连续性检查和独立最终视觉 QA。重做后的左向观察帧已确认朝屏幕左侧；枪身在观察方向中保持笔直。

`pet.json` 与 `spritesheet.webp` 是安装文件；`source/hanli-jiedan-peak-20260928-production` 保存生成输入、中间产物与完整 QA 证据。
