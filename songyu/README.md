# 宋玉（Songyu）

一款适用于 Codex Desktop 的《凡人修仙传》动漫宋玉人形动态宠物。

造型采用适合桌面小尺寸显示的 Q 版中国 3D 动漫风格，保留宋玉的青白渐变仙裙、白玉发冠、侧边玉饰、深色长发与温柔眉眼。鼠标悬停触发她的标志性吹茶动作；左右拖动时，她会结印御空飞行，发丝、衣袖和裙摆随飞行方向自然后扬，不使用遁光球。

![宋玉吹茶动画](assets/jumping.gif)

## 特点

- 《凡人修仙传》动漫宋玉人形造型
- 青白仙裙、白玉发冠与深色长发
- `jumping` 自定义为五帧吹茶循环
- 左右移动为结印御空飞行，无光球、光尾和速度线
- 9 套 Codex 标准状态动画
- 16 个顺时针观察方向
- Codex Pet Sprite v2 格式
- 透明背景 WebP 图集

## 动作总览

![宋玉完整动作总览](assets/contact-sheet.png)

| 状态 | 效果 |
| --- | --- |
| `idle` | 呼吸、眨眼与发丝微动 |
| `running-right` | 结印向右御空飞行，衣袂向左后扬 |
| `running-left` | 结印向左御空飞行，衣袂向右后扬 |
| `waving` | 温柔挥手问候 |
| `jumping` | 鼠标悬停：端杯、抬杯、吹茶、收势眨眼 |
| `failed` | 低头失落的失败反馈 |
| `waiting` | 等待确认或用户输入 |
| `running` | 专注处理任务 |
| `review` | 审阅任务结果 |
| Look directions | 16 个鼠标观察方向 |

![宋玉向右飞行动画](assets/running-right.gif)

![宋玉向左飞行动画](assets/running-left.gif)

## 安装

在仓库根目录执行 PowerShell：

```powershell
$target = Join-Path $HOME ".codex\pets\songyu"
New-Item -ItemType Directory -Path $target -Force | Out-Null
Copy-Item .\songyu\pet.json, .\songyu\spritesheet.webp -Destination $target -Force
```

复制完成后重启 Codex Desktop，然后在 pet 选择界面中选择“宋玉”。

## 文件结构

```text
songyu/
|-- README.md
|-- pet.json
|-- spritesheet.webp
|-- assets/
|   |-- contact-sheet.png
|   |-- idle.gif
|   |-- jumping.gif
|   |-- running-left.gif
|   |-- running-right.gif
|   `-- waving.gif
`-- source/
    `-- songyu-20260723/   # 生成输入、中间文件与完整 QA 证据
```

## 图集规格与验证

| 项目 | 数值 |
| --- | --- |
| Sprite 版本 | 2 |
| 图集尺寸 | 1536 × 2288 |
| 网格 | 8 列 × 11 行 |
| 单帧尺寸 | 192 × 208 |
| 格式 | RGBA WebP |

最终图集已通过 Codex v2 图集验证、逐行动作检查、方向语义检查、三份隔离盲测、连续性检查与最终视觉 QA。连续性检测对正下和正上两个跨行连接给出轻微差异提醒，经正常尺寸循环复核后确认没有明显跳变。

## 说明

`pet.json` 和 `spritesheet.webp` 是 Codex Desktop 安装所需的发布文件；`source/songyu-20260723` 保存可追溯的生成输入、中间产物和 QA 证据，不参与日常安装。
