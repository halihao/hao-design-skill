# JoJoMath Design Skill

这个仓库用于团队共同维护 `jojomath-design` Codex skill。它沉淀 JoJoMath 的产品设计原则、业务主链路、UI 设计规范、宣传视觉规范、案例库和 QA 检查清单。

## 目录结构

```text
jojomath-design/
├── SKILL.md
├── agents/
│   └── openai.yaml
├── references/
│   ├── product-principles.md
│   ├── business-flows.md
│   ├── design-system.md
│   ├── ui-patterns.md
│   ├── marketing-visuals.md
│   ├── examples.md
│   └── qa-checklist.md
└── assets/
    ├── brand/
    ├── screenshots/
    ├── figma-exports/
    └── marketing-examples/
```

## 团队如何使用

把仓库拉到本地后，将 `jojomath-design` 目录复制到 Codex 的 skills 目录：

```bash
mkdir -p ~/.codex/skills
cp -R jojomath-design ~/.codex/skills/
```

重新打开 Codex 或新建对话后，可以这样使用：

```text
使用 jojomath-design 设计一个 JoJoMath 学生做题页
使用 jojomath-design 检查这张宣传图是否符合 JoJoMath 规范
使用 jojomath-design 设计一张 JoJoMath 暑期课程宣传图
```

## 维护方式

- 新增产品截图：放到 `jojomath-design/assets/screenshots/`
- 新增 Figma 导出图：放到 `jojomath-design/assets/figma-exports/`
- 新增宣传图案例：放到 `jojomath-design/assets/marketing-examples/`
- 新增品牌资产：放到 `jojomath-design/assets/brand/`
- 每新增一个案例，都要同步更新 `jojomath-design/references/examples.md`
- 规范变化要优先更新 `references/`，不要只改口头说明

## 发布建议

建议把 `main` 分支作为团队认可版本。修改规范时新建分支，提交 PR，由产品、设计或负责人确认后合并。
