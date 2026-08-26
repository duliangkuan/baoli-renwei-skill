# 暴力人味 Skill

一个用于减少中文 AI 草稿模板腔、恢复作者表达并保留原意的 Agent Skill。

它会优先处理空泛开场、机械排比、模糊归因、过度工整的句式、同义反复和没有信息量的结尾。它不是简单替换同义词，也不承诺规避任何 AI 检测系统。

## 安装

```bash
npx skills add https://github.com/duliangkuan/baoli-renwei-skill.git
```

也可以手动克隆：

```bash
git clone https://github.com/duliangkuan/baoli-renwei-skill.git ~/.agents/skills/baoli-renwei
```

## 使用示例

```text
调用“暴力人味 Skill”编辑 demo/original.md。

保留原有观点和信息，不新增事实、数据与引用；处理模板化过渡、空泛判断、机械排比和同义反复；保持正式语气；输出修改稿和修改说明。
```

仓库内提供了一组约 500 字的模拟论文片段：

- `examples/original.md`：故意保留常见 AI 模板腔的原稿
- `examples/revised.md`：使用 Skill 润色后的版本
- `examples/change-log.md`：主要问题与修改说明

## 使用边界

- 适用于用户有权编辑的草稿、文章、脚本和说明文档。
- 不虚构事实、数据、引用、案例或个人经历。
- 学术文本的研究、论证与引用应由作者本人负责，并遵守学校、期刊及机构对 AI 辅助写作的披露要求。
- AI 文本检测结果存在误判，只能作为观察指标，不能证明文本的真实作者，也不应作为本 Skill 的效果承诺。

## 来源与许可

本 Skill 重新组织并精简了中文写作编辑规则，设计受到以下项目启发：

- [blader/humanizer](https://github.com/blader/humanizer)
- [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh)
- [Wikipedia: Signs of AI writing](https://en.wikipedia.org/wiki/Wikipedia:Signs_of_AI_writing)

上述两个代码仓库均采用 MIT License。本仓库保留相关著作权声明，并以 MIT License 发布。
