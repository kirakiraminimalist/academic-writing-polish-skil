# Academic Writing Polish

面向中英文学术论文的清晰表达 skill：减少模板腔和重复，补齐主语，保留原意、数据、引用与研究边界。

本项目将论文反复润色中的编辑经验整理为可复用流程。它不是检测器规避工具，不保证AIGC分数下降，不生成虚假研究数据或文献。AGI通常指通用人工智能，本文所说的论文检测场景是AIGC。

## 安装

下载本仓库，将含有 `SKILL.md` 的目录保存为 `academic-writing-polish`，放入所用工具的 skills 目录。Codex默认路径为 `~/.codex/skills/academic-writing-polish`。

若使用支持GitHub仓库安装的 skills CLI，可运行以下命令：

```bash
npx skills add https://github.com/kirakiraminimalist/academic-writing-polish-skil --skill academic-writing-polish
```

安装后重新打开会话，或按工具要求刷新技能。

## 使用

```text
使用 $academic-writing-polish 润色以下中文论文小节。
保持中文，保留论点、数据、引用编号与专业术语。
输出修改后的正文和关键修改说明，无法核实的信息单列。
【粘贴小节原文】
```

支持逐段润色、修改前后对照和结合用户提供的AIGC报告定位修改。Word标黄、格式保持与PDF校验依赖运行环境的文档能力，skill本身不包含Word渲染器。

## 边界

- 不将仿真结果写成现场业绩，不把相关性改成因果关系。
- 不编造数据、引用或作者经历，不删除必要的限定条件。
- 不自动上传论文或调用第三方检测服务。
- 示例为合成演示，不包含个人论文、企业内部数据或真实检测记录。
- 作者应核对全部结果，并遵守所在机构关于AI辅助写作与披露的规定。

## 验证范围

可使用 Codex skill-creator 的 `quick_validate.py` 检查技能结构。结构校验通过不等于学术内容已经核实，也不代表任何检测分数承诺。
