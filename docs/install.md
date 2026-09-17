# 安装与更新

[English](install.en.md)

## 适用 Agent

豆包桌面端（本地 Skills 模式）、WorkBuddy、Claude Code、Codex，以及其他支持 Skills 的 Agent。按所用客户端选择下面的安装方式。

## 快速安装

Codex、Claude Code 等安装器已列出的 Agent，可在终端执行，需要 Node.js 和 `npx`：

```bash
npx -y skills add ZanePan2027/zane-career-skills -g --skill "*"
```

这会安装完整求职工具箱。`--skill "*"` 选择全部 Skills；在安装器中选择目标 Agent，安装后按客户端要求重载。只在当前项目使用时，省略 `-g`。

也可以直接告诉 Agent：

```text
请从 https://github.com/ZanePan2027/zane-career-skills 安装全部 Skills，
然后使用 zane-career-assets，帮我处理这件事：……
```

## 豆包与 WorkBuddy

在这两个客户端中，直接发送上面的 Agent 安装请求，并说明正在使用哪个客户端。

| 客户端 | 安装位置与操作 |
| --- | --- |
| WorkBuddy | 让 Agent 将仓库 `skills/` 下的各个 Skill 文件夹安装到用户目录的 `.workbuddy/skills/`，保留每个文件夹中的完整内容。安装后到「专家·技能·连接器 → 技能 → 我安装的」查找 `zane-career-assets` 并启用。 |
| 豆包 macOS 本地 Skills 模式 | 让 Agent 将各个 Skill 文件夹安装到 `~/.agents/skills/`，然后在该客户端的本地 Skills 模式中重新加载。 |

若安装器的列表没有这两个名字，直接采用上述方式。安装后的入口应为 `<技能目录>/zane-career-assets/SKILL.md`，不要在技能目录中再套一层仓库文件夹。新建对话后说“使用 zane-career-assets，帮我……”，开始第一件事。

## 开始使用

日常从 `zane-career-assets` 进入，提供当前任务与手边材料。可以先整理一段经历、比较两个岗位、写一段简历，或练习面试。看[完整使用示例](guide.md)。

## 更新与保存

告诉 Agent：“比较这个仓库与我安装的版本，保留我的本地修改后更新走出象牙塔。”更新时核对实际文件与修订，不只看版本号。

Skill 安装目录保存方法。单次任务无需建立目录；需要保存个人材料时沿用当前项目，位置已知不重复询问。个人文件不放进Skill安装目录。

[返回首页](../README.md)
