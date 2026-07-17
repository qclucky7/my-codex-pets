# 云珩（Yunheng）

一款适用于 Codex Desktop 的中国古风动态宠物。

云珩是一位白发月白仙袍、气质清冷俊雅的年轻仙君。鼠标悬停时，他会单手掐诀，召出一条白色东方龙在身后盘旋。

![云珩白龙悬停动画](assets/hover-dragon.gif)

## 特点

- 中国古风仙侠人物设计
- 白发、月白与淡青色层叠仙袍
- 鼠标悬停：单手掐诀，白龙绕身显现
- 鼠标方向追踪：16 个观察方向
- 包含 Codex 宠物所需的 9 套标准动画
- Codex Pet Sprite v2 格式
- 透明背景 WebP 图集

## 动作总览

![云珩完整动作总览](assets/contact-sheet.png)

图集包含以下状态：

| 状态 | 效果 |
| --- | --- |
| `idle` | 待机、轻微呼吸与衣摆摆动 |
| `running-right` | 向右拖动 |
| `running-left` | 向左拖动 |
| `waving` | 挥手动作 |
| `jumping` | 鼠标悬停：掐诀并召唤白龙 |
| `failed` | 任务失败反馈 |
| `waiting` | 等待确认或用户输入 |
| `running` | Codex 正在工作 |
| `review` | 审阅任务结果 |
| Look directions | 16 个鼠标观察方向 |

## 安装

### Windows PowerShell

在仓库根目录执行：

```powershell
$target = Join-Path $HOME ".codex\pets\yunheng"
New-Item -ItemType Directory -Path $target -Force | Out-Null
Copy-Item .\pet.json, .\spritesheet.webp -Destination $target -Force
```

也可以手动将下面两个文件复制到：

```text
C:\Users\<你的用户名>\.codex\pets\yunheng\
```

需要复制的文件：

```text
pet.json
spritesheet.webp
```

复制完成后重启 Codex Desktop，然后在宠物选择界面中选择“云珩”。

## 文件结构

```text
yunheng/
├── README.md
├── pet.json
├── spritesheet.webp
├── assets/
│   ├── hover-dragon.gif
│   └── contact-sheet.png
└── source/
    └── yunheng-20260716/   # 完整生成、分帧、提示词与 QA 工程
```

## 图集规格

| 项目 | 数值 |
| --- | --- |
| Sprite 版本 | 2 |
| 图集尺寸 | 1536 × 2288 |
| 网格 | 8 列 × 11 行 |
| 单帧尺寸 | 192 × 208 |
| 格式 | RGBA WebP |

最终图集已经通过 Codex v2 图集校验：无尺寸错误、空帧错误或透明背景错误。

## 说明

`pet.json` 和 `spritesheet.webp` 是普通用户安装宠物所需的文件；`source/yunheng-20260716` 是用于继续修改动作、重新组装图集和质量检查的完整工程，不参与日常安装。

上传 GitHub 前，请根据你希望采用的授权方式自行添加 `LICENSE` 文件。
