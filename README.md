# HD2 MODS 菜单适配技能

将 Helldivers 2 Lua 模组的可调参数接入 Bingus ModOptionsMenu 的 MODS 页面，包含开关、滑块、选项、配置保存和中英语言切换。

[阅读技能说明](SKILL.md) · [菜单接口参考](references/mod-options-menu.md) · [Lua 适配模板](assets/mods_menu_adapter.lua)

语言方案是在本模组首行放置 **Language**，提供 **简体汉字** 和 **English**，保存选择并翻译模组标题、参数标签及说明。当前菜单会将英文选项显示为 `ENGLISH`；应用后关闭并重新打开 Esc 菜单刷新文字。

将本仓库内容放入 `~/.codex/skills/hd2-mods-menu/`，使该目录直接包含 `SKILL.md`、`agents/`、`assets/` 和 `references/`。随后可使用 `$hd2-mods-menu` 调用。

使用示例：

> 使用 $hd2-mods-menu 将这个模组的可调参数接入 MODS 页面，并加入简体汉字和 English 语言选项。

技能格式和 Lua 模板已通过验证。实现参考 [爆裂铳初版破片 v0.1.1](https://github.com/abaabaaba234/hd2-eruptor-original-shrapnel/tree/v0.1.1)。
