# 仲神师

《凡人修仙传》动漫仲神师的精致中国 3D 动漫桌宠。采用正面成熟造型，参考乐上师的紧凑头身比例，较旧版减弱 Q 感。保留黑色巾帽与横簪、短须、双耳环、蓝灰法袍、金色肩纹和菱形胸饰。

角色自身右手持银色折扇，待机时展开轻轻扇风，配合呼吸和眨眼，左手自然垂放。其他状态按动作收拢或微开折扇，始终保持右手侧别。`jumping` 按用户要求保留双脚落地、左手掐指推演的循环，表情从凝神、皱眉思索变化到有所领悟，再回到平静。

## 预览

![正面待机扇扇子](assets/idle.gif)

![左手推演](assets/jumping.gif)

![完整联系表](assets/contact-sheet.png)

## 动作

| 状态 | 动作设计 |
| --- | --- |
| `idle` | 正面站立，右手持展开银扇轻扇，配合呼吸和眨眼，左手自然垂放 |
| `running-right` | 朝屏幕右侧直立滑行，脚部、袖摆与帽带交替变化，保持待机人物尺度 |
| `running-left` | 朝屏幕左侧短步行，伸步与双脚交会交替出现，保持长袍、人物尺度和折扇右手侧别 |
| `waving` | 左手轻挥致意，右手折扇稳定 |
| `jumping` | 双脚落地，左手掐指推演，眉眼与嘴角随思考变化 |
| `failed` | 推演受阻，眉眼低落，轻微垂首 |
| `waiting` | 期待回应的询问姿态 |
| `running` | 专注处理任务的克制思考姿态 |
| `review` | 凝神检查结果 |
| look directions | 下身与脚底位置稳定，眼睛、头颈和少量上身自然跟随 16 个顺时针方向，右手保持展开银扇 |

## 安装

在仓库根目录运行 PowerShell：

```powershell
$petId = "zhong-shenshi"
$target = Join-Path $HOME ".codex\pets\$petId"
New-Item -ItemType Directory -Path $target -Force | Out-Null
Copy-Item ".\$petId\pet.json", ".\$petId\spritesheet.webp" -Destination $target -Force
```

安装目录只需 `pet.json` 与 `spritesheet.webp`。复制后重启 Codex Desktop，在 pet 选择界面选择仲神师。

## 格式与验证

- `spriteVersionNumber: 2`；图集 `1536 × 2288`，8 列 × 11 行，单元格 `192 × 208`。
- `pet.json` 的 `id` 与目录一致，图集使用相对路径 `spritesheet.webp`。
- `validate_atlas.py --require-v2` 通过，无错误或警告；未使用单元格透明。
- 单次确定性透明边缘处理通过，透明像素隐藏 RGB 残留为 0。
- 标准动作、方向语义、连续性和最终视觉 QA 均通过。
- 三组独立方向盲测采用严格多数，四个正方向全部通过；14 组轴向测试中没有硬性错误。
- 接受的轻微视觉说明：67.5°、112.5°、292.5°、315°、337.5° 的垂直线索在盲测中较轻，经有标签的完整方向环复核确认象限正确。157.5° → 180° 与 337.5° → 0° 的转头间距稍不均匀，没有明显尺度、身份或道具跳变。
- 展开银扇自然遮住部分胸饰；左移动时折扇微开。均保持同一银扇及右手侧别，面部可读。

## 源文件

2026-10-13 使用内置 imagegen 重做生产基本图及全部动作，使用 `hatch-pet` 脚本提取、组装和校验。用户批准的乐上师比例候选稿用于锁定设计，正式生产基本图另行生成并通过检查。最终 GIF 预览从完成单次透明边缘处理后的发布图集导出。

本次生产输入、完整提示词、未采用的生成结果、中间产物和 QA 证据保存在本地 `source/zhong-shenshi-20261013-front/`。各动作提示词在 `prompts/rows/`，生产基本图提示词为 `prompts/base-production.md`，最终报告为 `qa/run-summary.json`。旧版 `source/zhong-shenshi-20261012/` 保留，仓库配置默认不将 `source/` 纳入发布。
