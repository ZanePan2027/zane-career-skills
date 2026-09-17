# 验证范围 / Validation scope

1.0.0使用虚构材料和独立Agent执行检查。测试没有真实求职者、公司数据或平台账号。

## 实际检查

- 116项本地工程测试通过，其中11项验证可选求职状态工具：默认制作、指定暂停、按成果确认、修订失效、历史保留及旧状态兼容。
- 11个公开Skill结构验证、124个本地主入口发现及路由检查通过。结构正确不等于回答一定有效。
- 8次独立Agent执行：中文简历、BOSS资料与消息、负责人业绩和offer比较、无联网找岗、模拟面试首轮与独立续接、小型作品集、无旧简历的英文从零制作。
- 实际检查HTML简历和作品集渲染、手机显示、可编辑保存与链接。英文从零任务留下并渲染黑白线稿，再完成最终版。
- 首页中英文示意图实际渲染，安装命令、直接告诉Agent安装及本地文档链接检查。

## 发现与修正

旧版普通简历曾被中间确认阻断，所需HTML没有生成；本版默认直接制作候选。状态工具曾错误拦截不适用阶段，并在事实变化后缺少成果失效标记，已修正。

早期制作试跑保留了结构判断，却未留下实际黑白稿，不能证明执行了线稿步骤。随后明确要求新建／整体重设先生成可渲染线稿，并以“没有旧简历的英文制作”独立测试。前期用例未全部在最终措辞下重跑。原有英文文风、PDF排版与双语对应方法经版本对照保留，但本轮没有重新验证全部格式与语言。

生成包发现继承本地隐藏属性，已在构建时清理副本属性并重验。最终发布另检查公开内容、提交身份和线上文件一致性。

## 没有验证的内容

没有真实BOSS账号操作、发送或投递；没有招聘者评价、回复率、录用率、长期使用结果或不同模型对照。Word/PDF与复杂双语网站没有在本轮完整重跑。英文文风由Agent检查，未请真人母语招聘者评审。其他宿主及操作系统未逐一实测。

BOSS公开说明核查不证明所有客户端的字段限制、预览长度或附件能力。平台事实与未知见[核查记录](../skills/zane-career-assets/references/platform-evidence.md)。

Eight independent Agent executions used synthetic tasks. Engineering and artifact checks are not human hiring evaluations or comparative effectiveness evidence. Early runs were not all repeated after the final wording changes. A final English résumé task verified an actual rendered wireframe and editable result. No live recruiting account, real application, hiring outcome, full multilingual regression or cross-platform coverage is claimed.
