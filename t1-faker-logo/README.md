# Faker：T1 队标版

在原有 Faker Q 版形象的上衣胸前加入白色 T1 队标，主形象与九组动画同步更新。

- 透明原画：`final/faker.png`
- 桌宠清单、透明图集：`final/pet.json`、`final/spritesheet.webp`
- 九组动画预览：`qa/previews/`
- 57 帧动作一览：`qa/contact-sheet.png`
- 自动校验：`qa/review.json`、`final/validation.json`
- 视觉检查结果：`qa/visual-qa.json`

队标参照 [T1 官方素材页](https://www.t1.gg/community-1)及官网使用的队标图形，以白色置于黑色上衣胸前。全部视觉编辑使用内置 imagegen。向左移动单独编辑队标，未通过镜像生成，避免文字反转。

图集规格：1536 × 1872，8 列 × 9 行，每格 192 × 208；57 个使用格，15 个全透明空格。保留待机眨眼、左右移动、挥手、跳跃、失落、等待、工作中和检查结果九种状态。

原无队标版本已备份至上一级目录 `Faker-无队标备份.zip`。更新后的可分享文件为 `Faker-T1队标版.zip`，安装位置沿用 `%USERPROFILE%\.codex\pets\t1-faker`。

检查范围包括逐帧视觉、透明度、图集尺寸、空格和 GIF 时长；未在 Codex 桌宠运行界面内实测播放。
