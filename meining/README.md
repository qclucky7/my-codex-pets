# 梅凝（meining）

适用于 Codex Desktop 的《凡人修仙传》动漫梅凝 Q 版动态桌宠。

形象采用精致中国 3D 动漫 Q 版风格，保留中分双侧低髻、金铜叶片发饰、青绿宝石、垂珠耳坠、青白交领绣花长裙与深青腰封。角色约三头身，针对 `192 × 208` 桌宠单元格优化。

![梅凝动作总览](assets/contact-sheet.png)

## 动作

| 状态 | 效果 |
| --- | --- |
| `idle` | 轻微呼吸、眨眼与发梢袖摆变化 |
| `running-right` | 保持待机大小，向画面右侧移动 |
| `running-left` | 保持待机大小，向画面左侧移动 |
| `waving` | 温柔挥手 |
| `jumping` | 自定义为站定托脸动作，不跳跃 |
| `failed` | 低头、闭眼与轻微失落 |
| `waiting` | 摊手并期待用户确认或输入 |
| `running` | 站定思考并专注处理任务 |
| `review` | 托腮凝视并认真审阅 |
| Look directions | 16 个顺时针观察方向 |

![梅凝待机](assets/idle.gif)

![梅凝托脸](assets/jumping.gif)

![梅凝向右移动](assets/running-right.gif)

![梅凝向左移动](assets/running-left.gif)

## 安装

在仓库根目录执行 PowerShell：

```powershell
$target = Join-Path $HOME ".codex\pets\meining"
New-Item -ItemType Directory -Path $target -Force | Out-Null
Copy-Item .\meining\pet.json, .\meining\spritesheet.webp -Destination $target -Force
```

复制完成后重启 Codex Desktop，然后在 pet 选择界面中选择“梅凝”。

## 图集规格

| 项目 | 数值 |
| --- | --- |
| Sprite 版本 | 2 |
| 图集尺寸 | 1536 × 2288 |
| 网格 | 8 列 × 11 行 |
| 单帧尺寸 | 192 × 208 |
| 格式 | RGBA WebP |

发布文件为 `pet.json` 与 `spritesheet.webp`；`source/meining-20260727/` 保存生成输入、中间产物和完整 QA 证据。
