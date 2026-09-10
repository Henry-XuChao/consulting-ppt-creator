# Consulting PPT Creator

一个用于创建、改造并视觉质检专业咨询风格 PowerPoint 演示文稿的 Codex Skill。它采用克制的白、黑、绿色视觉语言，强调清晰的叙事、结论导向的标题、可编辑的原生元素与完整的视觉检查。

> 本项目为独立维护的开源 Skill，不附带任何第三方品牌的官方模板、Logo、专有字体或品牌资产。

## 主要功能

- 创建面向管理层、客户或项目团队的专业咨询风格 PPT。
- 将现有演示文稿重新设计为简洁、结论优先的咨询视觉风格。
- 基于“背景 → 问题 → 证据 → 影响 → 建议 → 行动”的叙事组织内容，并为每页设置一个明确观点。
- 使用白色主画布、黑色文字和克制的绿色强调，避免密集卡片、过度装饰和不必要的渐变。
- 优先生成可编辑的原生文本、图表、表格和形状；在需要时使用具有编辑感的配图。
- 在交付前渲染并检查每一页，修复文字溢出、元素重叠、层级不清、排版不一致和未替换的占位内容。
- 支持用户提供的获授权模板、Logo、字体和品牌规范；这些官方资产优先于本 Skill 的默认视觉规则。

## 安装方法

### 前置条件

- 已安装并可使用 Codex。
- 已具备 `presentations:Presentations` skill。该 Skill 负责 PPTX 的创建、渲染和视觉质量检查。

### 从 GitHub 安装

将仓库克隆到本地后，把 skill 目录复制到 Codex skills 目录：

```powershell
git clone https://github.com/<your-account>/consulting-ppt-creator.git
Copy-Item -Recurse -Force .\consulting-ppt-creator "$env:USERPROFILE\.codex\skills\consulting-ppt-creator"
```

重启 Codex 或开启一个新会话后即可加载。调用示例：

```text
使用 $consulting-ppt-creator，为一家制造企业制作一份 10 页的供应链转型建议书。
```

### 使用官方资产

如果你拥有获授权的模板或品牌资产，请在请求中附上它们。Skill 会以这些资产为唯一视觉依据；请勿将没有授权的模板、Logo 或字体提交到本仓库。

## 文档结构

```text
consulting-ppt-creator/
├── SKILL.md
│   └── Skill 的触发条件、内容策略、设计流程、交付与视觉质检要求。
├── agents/
│   └── openai.yaml
│       └── Codex 中的显示名称、简要介绍及默认调用提示。
└── references/
    └── brand-system.md
        └── 默认的咨询演示视觉系统：色彩、字体、版式、页面原型、图像和品牌资产使用边界。
```

## 使用原则

- 仅在用户未提供获授权模板或品牌包时使用默认视觉系统。
- 不生成、重绘、仿制或拼接第三方 Logo；不把输出描述为任何第三方的官方模板。
- 研究型事实应保留来源；用户提供的事实、外部来源和推断应清晰区分。
- 每份演示稿交付前均应完成渲染与逐页视觉检查。

## 许可证

在公开发布前，请为本项目添加许可证文件。若全部内容均由你原创且希望他人自由使用与修改，可采用 [MIT License](https://choosealicense.com/licenses/mit/)。
