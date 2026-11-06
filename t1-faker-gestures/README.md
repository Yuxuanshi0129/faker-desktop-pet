# Faker 桌宠：嘘与点赞版

按已确认的选择替换两组动作：

| 原动作 | 新动作 | 帧数 |
| --- | --- | --- |
| 等待输入 | 食指贴在嘴前比嘘，伴随轻微呼吸和眨眼 | 6 |
| 挥手 | 经典竖大拇指，伴随小幅抬手和点头 | 4 |

其余七组动作与替换前图集逐像素一致。新动作沿用现有 Faker 形象、红黑队服和白色 T1 队标。

桌宠仍有九组状态、57 帧，透明图集规格为 1536 × 1872，每格 192 × 208。`waiting` 与 `waving` 是对应的新动作所使用的应用状态名。

- 桌宠文件：`final/pet.json`、`final/spritesheet.webp`
- 嘘动画预览：`qa/previews/waiting.gif`
- 点赞动画预览：`qa/previews/waving.gif`
- 全部动作一览：`qa/contact-sheet.png`
- 校验：`final/validation.json`、`qa/review.json`、`qa/row-preservation.json`
- 视觉复查：`qa/visual-qa.json`

两组新动作使用内置 imagegen 分别生成，透明图集通过确定性切帧与合成导出。GIF 预览保留专用透明色，避免将几乎透明的边缘显示成彩色杂点。

安装位置沿用 `%USERPROFILE%\.codex\pets\t1-faker`，新版安装包为上一级目录的 `Faker-嘘与点赞桌宠.zip`。替换前版本备份为 `Faker-替换嘘和点赞前备份.zip`。

验证覆盖图集尺寸、帧数、透明度、保留动作的逐像素一致性及新动作的帧序列和时长；未在 Codex 桌宠运行界面内实测播放。
