# AGENTS.md

## 项目定位

本仓库用于集中保存、维护和发布个人 Codex Desktop pets。每只 pet 使用一个独立的顶层目录；不要把 pet 的发布文件直接放在仓库根目录。

处理 pet 的新建、修复、升级、校验或打包任务时，必须先使用已安装的 `hatch-pet` skill，并遵循其 v2 工作流与 QA 要求。仅修改文档或仓库配置时，不需要重新生成图像。

## 目录约定

```text
<pet-id>/
|-- README.md
|-- pet.json
|-- spritesheet.webp
|-- assets/
|   |-- contact-sheet.png
|   `-- *.gif
`-- source/
    `-- <pet-id>-YYYYMMDD/
```

- `<pet-id>` 使用小写 ASCII kebab-case，并与 `pet.json` 中的 `id` 完全一致。
- `pet.json` 和 `spritesheet.webp` 是安装所需的发布文件，必须同时存在。
- `assets/` 保存 README 展示用的联系表、动画预览等精选产物。
- `source/` 保存可追溯的生成输入、中间产物与 QA 证据。除非用户明确要求清理，否则不要删除已有源文件或 QA 记录。
- 每只 pet 的具体说明写在自己的 `README.md`；根 README 只维护仓库级说明和 pet 索引。

## Codex Pet v2 合同

所有新 pet 均使用 `spriteVersionNumber: 2`：

- 图集：`1536 x 2288`，8 列 x 11 行。
- 单元格：`192 x 208`。
- 行 0-8：`idle`、`running-right`、`running-left`、`waving`、`jumping`、`failed`、`waiting`、`running`、`review`。
- 行 9-10：16 个顺时针 look directions。
- 未使用的单元格必须完全透明。
- `spritesheetPath` 使用相对路径 `spritesheet.webp`。

不要手工拼接、拉伸或逐格修补最终图集。视觉生成使用 `imagegen`，图集组装、透明背景处理和校验使用 `hatch-pet` 提供的确定性脚本。

## 修改规则

- 保留用户已有改动，不覆盖与当前任务无关的文件。
- 不要重新编码或批量改写二进制图像。
- JSON 文件使用 UTF-8、两个空格缩进，并以换行结尾。
- Markdown 使用 UTF-8，链接优先使用相对路径，确保在 GitHub 上可浏览。
- 修改 pet 身份、动作、图集或元数据时，同步检查该 pet 的 README 和根 README 索引。
- 未经用户明确要求，不把开发中间文件复制到 `~/.codex/pets`，也不替用户发布或推送仓库。

## 完成前检查

1. `pet.json` 可解析，且 `id` 与目录名一致。
2. `spriteVersionNumber` 为 `2`，`spritesheetPath` 指向存在的文件。
3. v2 图集通过 `hatch-pet` 的 `validate_atlas.py --require-v2` 校验。
4. 对新建或修复的 pet，确定性校验、方向语义、盲测、连续性与最终视觉 QA 均已完成。
5. 根 README 中的 pet 索引与仓库实际目录一致。
6. 仅提交必要文件，并在交付说明中列出验证结果。
