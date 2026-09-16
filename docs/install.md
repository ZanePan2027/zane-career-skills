# 安装与更新

在支持 Agent Skills 的工具中使用这套方法。[English](install.en.md)

## 快速安装

在终端执行，需要 Node.js 和 `npx`：

```bash
npx -y skills add ZanePan2027/zane-career-skills -g --all
```

这会安装完整求职工具箱。按安装界面选择 Agent，安装后按宿主要求重载。只在当前项目使用时，省略 `-g`。

也可以直接告诉 Agent：

```text
请从 https://github.com/ZanePan2027/zane-career-skills 安装全部 Skills，
然后使用 zane-career-assets，帮我处理这件事：……
```

## 开始使用

日常从 `zane-career-assets` 进入，提供当前任务与手边材料。可以先整理一段经历、比较两个岗位、写一段简历，或练习面试。看[完整使用示例](guide.md)。

## 更新与保存

告诉 Agent：“比较这个仓库与我安装的版本，保留我的本地修改后更新走出象牙塔。”更新时核对实际文件与修订，不只看版本号。

Skill 安装目录保存方法。个人经历、求职材料和接续记录放在你选择的项目文件夹中；继续任务时提供该位置。

[返回首页](../README.md)
