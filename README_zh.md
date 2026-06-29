# Dylan's Agent Skills (Dylan 的智能体技能包)

一个专为 AI 编程智能体（如 **Claude Code**、**Gemini**、**Cursor** 和 **Windsurf**）设计的高质量、可重用的 **Skills（技能包）** 集合。这些技能旨在为你的 AI 助手配备在产品设计、Apple 开发基础设施以及美学转化方面的专业工作流。

本仓库完全兼容 **[skills.sh](https://skills.sh)** —— AI 智能体行为的包管理器和注册表。

---

## 🚀 快速开始（安装）

你可以使用 `skills.sh` 方便地直接从 GitHub 将这些技能安装到你的项目或全局环境中。

### 1. 安装本仓库中的所有技能
将本仓库中所有可用的技能安装到当前项目：
```bash
npx skills add enzoding/dylan_skills
```

### 2. 安装特定技能
如果你只需要某一个特定技能（例如 `classic-braun-design`）：
```bash
npx skills add enzoding/dylan_skills --skill classic-braun-design
```

### 3. 全局安装
要使技能在你的所有项目中均可用，请在命令末尾添加 `-g` 参数：
```bash
npx skills add enzoding/dylan_skills --skill classic-braun-design -g
```

### 4. 更新技能
要检查并拉取已安装技能的最新更新，请运行：
```bash
npx skills update
```

---

## 🗂️ 技能目录（分类归档）

以下是本仓库中可用技能的分类列表：

### 🎨 设计与美学 (Design & Aesthetics)
*专注于视觉润色、艺术指导以及将物理或产品设计哲学转化为数字 UI 的技能。*

| 技能名称 | 触发词 / 何时使用 | 描述 |
| :--- | :--- | :--- |
| **[classic-braun-design](./classic-braun-design)** | 当要求 Braun、Dieter Rams（迪特·拉姆斯）风格、复古计算器/时钟 UI 时 | 将博朗（Braun）经典的物理产品设计语言转化为响应式的数字 UI。 |
| **[less-but-better-design](./less-but-better-design)** | 极简主义、克制、良好审美审计相关的通用请求 | 关于纯粹、功能性且经久耐用的产品设计美学的更广泛指导。 |
| **[object-to-design](./object-to-design)** | 将任何物理品牌（如 Nothing、Dyson、Apple、Brompton 等）转化为 UI | 从经典的工业实体对象中创建开箱即用的 `DESIGN.md` 设计 Token 和布局规范。 |

### 🛠️ 工具与基础设施 (Tooling & Infrastructure)
*用于自动化复杂技术管线、环境搭建和开发运维的工作流技能。*

| 技能名称 | 触发词 / 何时使用 | 描述 |
| :--- | :--- | :--- |
| **[asc-signing-setup](./asc-signing-setup)** | iOS/macOS 包名（Bundle ID）、证书轮转、描述文件（Provisioning Profiles）配置 | 使用 App Store Connect 命令行工具（`asc`）快速配置安全的签名同步、Capabilities 以及证书。 |
