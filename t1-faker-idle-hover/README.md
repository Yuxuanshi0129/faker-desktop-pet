# Faker：默认嘘，悬停点赞

已按最终要求设置：

- 默认空闲和静态首帧：食指贴嘴的“嘘”姿势。
- 鼠标移到桌宠上：竖大拇指。
- 鼠标移开：回到默认姿势；任务活动提示仍由应用选择对应状态。

已读取本机应用 26.930.3930.0 的桌宠组件，并用该组件的实际代码验证：指针进入时选用 `jumping`，离开时恢复基础状态，基础默认状态是 `idle`。因此本版将嘘放入 `idle` 的 6 帧，将点赞放入 `jumping` 的 5 帧。点赞末帧使用已批准的起始帧完成闭环；没有重新生成角色。

之前放进等待输入和挥手的动作已恢复原版，本次更改的是默认与悬停所对应的两个槽位。

- 默认预览：`qa/previews/idle.gif`
- 悬停预览：`qa/previews/jumping.gif`
- 静态原画：`final/faker.png`
- 悬停表情原画：`final/faker-hover.png`
- 桌宠文件：`final/pet.json` 与 `final/spritesheet-idle-hover.webp`
- 触发验证：`qa/pointer-behavior-test.json`

图集仍为 1536 × 1872，9 组状态、57 帧、15 个透明空格。使用新的图片文件名以避免沿用旧纹理缓存。

安装目录：`%USERPROFILE%\.codex\pets\t1-faker`。如果正在运行的桌宠仍显示旧图，到设置 → Pets 点击 Refresh，再选择 Faker。

刷新操作依据：[官方 Pets 说明](https://learn.chatgpt.com/docs/pets)。
