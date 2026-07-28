# 元瑶（Yuanyao）

一款适用于 Codex Desktop 的《凡人修仙传》动漫元瑶动态宠物。

元瑶采用适合桌面小尺寸显示的精致中国 3D 动漫 Q 版造型：冷白肤色、蓝紫瞳、黑色超长直发、环形编发与细侧辫，搭配深朱红交领外衣、黑色内裙、银色圆形腰饰和红黑半透明轻纱。整体气质清冷、神秘而克制。

![元瑶待机动画](assets/idle.gif)

## 特点

- 《凡人修仙传》动漫元瑶角色造型
- 约三头身的精致中国 3D 动漫 Q 版风格
- 黑色长发、蓝紫瞳、环形编发与红黑轻纱长裙
- 9 套 Codex 标准状态动画
- 16 个顺时针观察方向
- Codex Pet Sprite v2 格式
- 透明背景 WebP 图集

## 动作总览

[查看元瑶完整动作总览](assets/contact-sheet.png)

| 状态 | 效果 |
| --- | --- |
| `idle` | 呼吸、眨眼与发丝轻摆 |
| `running-right` | 向右拖动移动，长发与轻纱自然跟随 |
| `running-left` | 向左拖动移动，保持正确朝向与交替步态 |
| `waving` | 克制而自然的挥手问候 |
| `jumping` | 专属轻盈旋身、拂袖与回望动作，不采用普通跳跃 |
| `failed` | 低头收势的失落反馈 |
| `waiting` | 安静等待确认或用户输入 |
| `running` | 专注处理任务 |
| `review` | 凝神审阅任务结果 |
| Look directions | 16 个顺时针观察方向 |

![元瑶挥手动画](assets/waving.gif)

![元瑶专属悬停动作](assets/jumping.gif)

![元瑶向右移动动画](assets/running-right.gif)

## 安装

在仓库根目录执行 PowerShell：

```powershell
$target = Join-Path $HOME ".codex\pets\yuanyao"
New-Item -ItemType Directory -Path $target -Force | Out-Null
Copy-Item .\yuanyao\pet.json, .\yuanyao\spritesheet.webp -Destination $target -Force
```

复制完成后重启 Codex Desktop，然后在 pet 选择界面中选择“元瑶”。

## 文件结构

```text
yuanyao/
|-- README.md
|-- pet.json
|-- spritesheet.webp
|-- assets/
|   |-- contact-sheet.png
|   |-- idle.gif
|   |-- jumping.gif
|   |-- running-right.gif
|   `-- waving.gif
`-- source/
    `-- yuanyao-20260727/   # 生成输入、中间文件与完整 QA 证据
```

## 图集规格与验证

| 项目 | 数值 |
| --- | --- |
| Sprite 版本 | 2 |
| 图集尺寸 | 1536 × 2288 |
| 网格 | 8 列 × 11 行 |
| 单帧尺寸 | 192 × 208 |
| 格式 | RGBA WebP |

最终图集已通过 Codex v2 图集验证、逐行动作检查、方向语义检查、三份隔离盲测、连续性检查与最终视觉 QA。方向 `067.5°` 和 `112.5°` 的垂直线索较轻，但在正常尺寸的有序循环中保持正确象限；修复后的 `270° → 292.5° → 315° → 337.5°` 始终保持同一左侧脸并连续仰视，没有翻面。

## 说明

`pet.json` 和 `spritesheet.webp` 是安装所需的发布文件；`source/yuanyao-20260727` 保存可追溯的生成输入、中间产物和 QA 证据，不参与日常安装。
