# Faker 桌宠素材合集（fan-made / 非官方）

一个用 ChatGPT / Codex 内置 imagegen 生成的 Q 版「Faker」桌宠素材合集，包含制作各阶段的版本、动画图集、预览 GIF、生成提示词与校验记录。

> ⚠️ **非官方同人作品**：本项目与 Lee "Faker" Sang-hyeok 本人、T1、Riot Games 及任何赞助商均无关联，未获授权或背书。部分版本胸前带有手绘的战队风格标记，仅为同人二创，不代表官方身份。所有商标、肖像权归各自权利人所有。本项目仅供个人学习与展示，不作商业用途。

## 仓库内容

| 路径 | 说明 |
| --- | --- |
| `t1-faker/` | 主版本：默认「嘘」、鼠标悬停「点赞」 |
| `t1-faker-idle-hover/` | 悬停动作替换的中间版本 |
| `t1-faker-gestures/` | 等待 / 挥手替换为嘘 / 点赞的版本 |
| `t1-faker-logo/` | 胸前加入白色战队风格标记的 Q 版 |
| `faker-emotes/` | 嘘 / 点赞两张静态表情原画与预览 |
| `t1-logo-assets/` | 制作时参考的第三方网页快照与矢量素材 |
| `Faker-*.zip` | 各阶段可直接安装或分享的打包文件 |
| `Faker-*.md`、`t1-faker-discovery.md` | 生成提示词、动作替换提示词、角色考据与来源 |

每个版本目录的 `final/` 内含 `pet.json` 与 `spritesheet*.webp`，`qa/previews/` 内含各状态 GIF 预览，`qa/` 内含逐帧校验记录。

## 直接使用

任一版本 `final/` 目录内：

- `pet.json`：id / 显示名 / 描述 / 图集文件名
- `spritesheet.webp`：1536 × 1872，8 列 × 9 行，每格 192 × 208，57 个使用格 + 15 个全透明空格，9 组状态

把该目录作为桌宠包放到 pets 目录，在「设置 → Pets」点 Refresh 并选择 Faker。参考官方说明：<https://learn.chatgpt.com/docs/pets>

## 动画状态

idle（默认 / 嘘）、running-right、running-left、waving、jumping（悬停 / 点赞）、failed、waiting、running、review。

## 隐私处理

仓库已移除 Python 虚拟环境与他人桌宠素材；把文档中的本机用户名路径泛化为 `%USERPROFILE%`；把第三方网页快照内嵌的 API key 替换为占位符。其余内容保持原样。

## 许可证

代码与文档：MIT，见 `LICENSE`。角色美术为同人二创，不适用 MIT 授权范围，权利归原权利人。
