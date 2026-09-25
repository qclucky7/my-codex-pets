# 凡人修仙传 Q 版桌宠

一个以《凡人修仙传》动漫角色为主题的 Codex Desktop Q 版动态桌宠合集。

项目采用统一的精致中国 3D 动漫 Q 版风格，在适配桌面小尺寸显示的同时，保留角色具有辨识度的发型、服饰、配色、饰品与性格化动作。每位角色都是一个可独立安装、维护和追溯的 pet，发布文件与生成/QA 工程放在同一目录中管理。

## 角色

| 角色 | 简介 | 格式 | 预览与说明 |
| --- | --- | --- | --- |
| 银月（`yinyue`） | 银发狐耳、异色瞳与月白短裙的灵动少女，悬停时模仿狐狸前爪 | Codex Pet Sprite v2 | [查看角色](yinyue/README.md) |
| 宋玉（`songyu`） | 青白仙裙、白玉发冠的温柔少女，悬停吹茶、拖动时结印御空飞行 | Codex Pet Sprite v2 | [查看角色](songyu/README.md) |
| 慕沛灵（`mupeiling`） | 橙红仙裙、温柔眉眼的古风少女，悬停时正面舒展双臂感受自由 | Codex Pet Sprite v2 | [查看角色](mupeiling/README.md) |
| 梅凝（`meining`） | 青白绣花长裙、金铜叶片发饰的温柔少女，悬停时站定托脸 | Codex Pet Sprite v2 | [查看角色](meining/README.md) |
| 元瑶（`yuanyao`） | 黑色长发、蓝紫瞳与红黑轻纱长裙的清冷少女，悬停时双手托脸、微微歪头 | Codex Pet Sprite v2 | [查看角色](yuanyao/README.md) |
| 紫灵（`ziling`） | 紫色眼眸、轻纱覆面与紫蓝仙裙的端庄少女，悬停时敛袖轻礼 | Codex Pet Sprite v2 | [查看角色](ziling/README.md) |
| 南宫婉（`nangong-wan`） | 银蓝发冠、额心红纹与蓝白仙裙的清雅少女，悬停时双手掐诀、双脚落地 | Codex Pet Sprite v2 | [查看角色](nangong-wan/README.md) |
| 乐上师（`yueshangshi`） | 青绿头纱、银色翠玉额饰与青绿银纹祭服的幕兰法士，展开双臂时保持双脚落地 | Codex Pet Sprite v2 | [查看角色](yueshangshi/README.md) |
| 韩立（`hanli`） | 青竹小轩时期的青绿竹纹长袍与沉静锐利眼神，悬停时持古卷推演阵法 | Codex Pet Sprite v2 | [查看角色](hanli/README.md) |
| 凌玉灵（`lingyuling`） | 灰白金星宫长袍、右侧弧形梳饰与清雅眉眼，悬停时正面双手比心 | Codex Pet Sprite v2 | [查看角色](lingyuling/README.md) |
| 南宫阙（`nangong-que`） | 黑色高髻、额心银白纹饰与蓝紫银纹长袍的冷静女修，悬停时双脚落地拂袖结印 | Codex Pet Sprite v2 | [查看角色](nangong-que/README.md) |
| 李缨宁（`liyingning`） | 双辫、灰白青绿侠装、佩剑与暖阳宝玉的灵秀少女，悬停时低头轻触宝玉 | Codex Pet Sprite v2 | [查看角色](liyingning/README.md) |

## 仓库结构

```text
my-codex-pets/
|-- AGENTS.md          # Codex 在本仓库中的开发与维护规则
|-- README.md          # 项目说明和 pet 索引
|-- LICENSE            # MIT License
`-- <pet-id>/
    |-- README.md      # 单只 pet 的介绍、预览和安装说明
    |-- pet.json       # Codex pet 元数据
    |-- spritesheet.webp
    |-- assets/        # 展示图与动画预览
    `-- source/        # 生成输入、中间文件与 QA 证据
```

后续《凡人修仙传》角色直接添加为新的顶层目录，例如 `hanli/`。目录名必须与 `pet.json` 的 `id` 一致，使用小写 ASCII kebab-case。

## 安装 pet

以 `mupeiling` 为例，在仓库根目录运行 PowerShell：

```powershell
$petId = "mupeiling"
$target = Join-Path $HOME ".codex\pets\$petId"
New-Item -ItemType Directory -Path $target -Force | Out-Null
Copy-Item ".\$petId\pet.json", ".\$petId\spritesheet.webp" -Destination $target -Force
```

复制完成后重启 Codex Desktop，然后在 pet 选择界面中选择对应角色。

安装目录中只需要：

```text
~/.codex/pets/<pet-id>/
|-- pet.json
`-- spritesheet.webp
```

## 统一风格

所有角色遵循同一套视觉方向：

- 精致中国 3D 动漫 Q 版造型，约三头身比例，适合桌面小尺寸辨识。
- 忠于《凡人修仙传》动漫角色的核心外观，不随意替换标志性发型、服装配色与饰品。
- 材质、光照、线条精细度、身体比例和面部表现保持系列一致。
- 动作符合角色性格与原作印象，并兼顾短循环动画的清晰度和连续性。
- 使用透明背景，不加入场景底图、文字、水印或与角色无关的装饰。

## 新增或维护角色

本仓库新增角色应来自《凡人修仙传》，并统一采用 Codex Pet Sprite v2：

- 8 列 x 11 行，单元格 `192 x 208`，完整图集 `1536 x 2288`。
- 前 9 行覆盖 Codex 标准状态动画，最后 2 行覆盖 16 个观察方向。
- `pet.json` 必须包含 `spriteVersionNumber: 2`。
- 发布前必须完成图集结构、透明背景、动作、方向语义、连续性和最终视觉 QA。

在 Codex 中创建或修改角色时，应使用项目的 [AGENTS.md](AGENTS.md) 约定和 `hatch-pet` 工作流。完成一只 pet 后：

1. 将 `pet.json` 与 `spritesheet.webp` 放到该 pet 的根目录。
2. 将精选预览放进 `assets/`，将可追溯工程放进 `source/`。
3. 编写该角色的 README，并更新本页的角色表格。
4. 验证元数据、文件路径和 v2 图集，确认 QA 无阻塞项。

## 许可协议

本项目使用 [MIT License](LICENSE)，是非官方粉丝创作项目，与原作版权方及动画制作方无隶属或授权关系。角色及作品相关权利归各自权利人所有；提交第三方参考图、字体、商标或其他素材前，请另行确认其授权允许纳入本仓库。
