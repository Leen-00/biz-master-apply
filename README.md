<div align="center">

# 🎓 biz-master-apply · 商科硕士 DIY 申请 Skill

**把整套留学申请流程固化成一个 AI 技能包** —— 选校、文书、CV、推荐信、面试、进度管理，
激活后直接对话即可，不用每次复制大段 Prompt。

<br>

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Status](https://img.shields.io/badge/Status-Active-success.svg)
![Target](https://img.shields.io/badge/Target-27fall%20%E5%95%86%E7%A7%91%E7%A1%95%E5%A3%B2-orange.svg)
![Language](https://img.shields.io/badge/Markdown-100%25-white.svg)

**适用方向**：金融 · 会计 · 商业分析 BA · 管理 · 经济 ｜ **适用人群**：DIY / 半 DIY 申请者

</div>

---

## ✨ 这个 Skill 能做什么

| 环节 | AI 帮你完成 | 对应文件 |
|---|---|---|
| 🔎 **选校定位** | 背景诊断、冲/稳/保分档、官网要求提取、同背景案例比对 | `references/school-selection.md` |
| ✍️ **PS / SOP 文书** | 素材脑暴 → 大纲 → 锁语气润色 → 招生官视角自检 | `assets/ps-outline.md` |
| 📄 **CV 简历** | 大白话经历改专业英文要点、对照项目要求优化 | `assets/cv-template.md` |
| 💌 **推荐信** | 沟通提纲、英文草稿框架、去 AI 味检查 | `assets/letter-rec.md` |
| 🎤 **面试准备** | AI 扮演严格面试官、行为面 / 专业面 / 简历追问题库 | `references/interview-questions.md` |
| 📬 **邮件套磁** | 简短直接的套磁 / 咨询邮件起草 | `assets/prompts.md` |
| 🗂 **进度管理** | 时间线倒排、材料清单核对、每周卡点复盘 | `assets/prompts.md` |

---

## 🗂 目录结构

```
biz-master-apply/
├── SKILL.md                  # 核心指令：元数据 + 工作原则 + 7 个环节流程
├── README.md                 # 本说明
├── LICENSE                   # MIT 许可证
├── .gitignore
├── assets/                   # 模板与可直接复制的 Prompt
│   ├── profile-template.md   # 个人背景填写模板
│   ├── prompts.md            # 全流程 Prompt 模板（选校/文书/CV/推荐信/面试/进度）
│   ├── ps-outline.md          # PS / SOP 五段大纲模板
│   ├── cv-template.md         # 申请 CV 结构模板
│   └── letter-rec.md         # 推荐信框架模板
└── references/               # 按需加载的详细参考
    ├── school-selection.md   # 选校评估维度与方法
    └── interview-questions.md # 商科面试题库与回答框架
```

---

## 🚀 快速开始

### 方式一：克隆到本地 Skill 目录（推荐）

```bash
git clone https://github.com/Leen-00/biz-master-apply.git
```

把整个 `biz-master-apply` 文件夹放进对应工具的 skills 目录：

| AI 工具 | Skill 目录位置 |
|---|---|
| **Claude Code** | 项目或用户目录下 `.claude/skills/` |
| **Kimi Code** | 按其 CLI 文档的 skills 目录 |
| **其他兼容 Agent Skills 的工具** | 参考各自文档的 skills 加载路径 |

### 方式二：下载 ZIP 解压

在仓库页面点 **`Code → Download ZIP`**，解压后把文件夹放入上述 skills 目录。

### 方式三：直接读取（不装目录也能用）

把 `SKILL.md` 内容作为系统 / 角色指令贴进对话，再按需引用 `assets/`、`references/` 里的文件即可。

---

## 💬 怎么用：直接说人话下指令

首次激活后，先按 `assets/profile-template.md` 填好个人背景发给 AI，然后直接说目标环节：

| 你想说 | AI 会做什么 |
|---|---|
| "帮我做选校定位，出冲稳保清单" | 诊断背景，分档并标注匹配理由与风险 |
| "基于我的素材出 PS 大纲" | 五段式大纲 + 每段要点，不直接写成文 |
| "把这段实习改成 CV 英文要点" | 动作动词开头、带工具与结果 |
| "扮演严格面试官，开始模拟面试" | 一问一答，作答后严格点评再追问 |
| "帮我倒排申请时间线" | 从入学日反推各环节节点与里程碑 |

> 各环节现成 Prompt 模板见 [`assets/prompts.md`](assets/prompts.md)。

---

## 🔒 工作原则（已写入 SKILL.md）

- 🚫 **不编造**：成绩、经历、数字、教授、课程、录取案例一律不虚构；不确定处标注"需核实"。
- 🚫 **不做保录承诺**，不把推测概率说成定论。
- ✍️ **文书三步法**：用户脑暴素材 → AI 出大纲 → 用户自写、AI 锁定语气润色。
- 🌐 **官网为准**：截止日期、先修课、学费、语言要求以院校官网当年信息为准。
- 🤝 **推荐信须推荐人知情确认**，不虚构与推荐人的互动。

---

## 🛠 自定义建议

- **填好固定背景**：把你的院校、GPA、语言、实习等直接写进 `SKILL.md` 第 1 节，省去每次重复。
- **补充专属案例**：按目标地区 / 方向在 `references/` 里加项目清单与录取案例。
- **保持主文件精简**：新增长模板放到 `assets/` 或 `references/`，`SKILL.md` 建议控制在 500 行以内。

---

## 📦 从本地推送到 GitHub（备查）

```bash
cd biz-master-apply
git init
git add .
git commit -m "feat: 商科硕士 DIY 申请全流程 Skill"
git remote add origin https://github.com/Leen-00/biz-master-apply.git
git branch -M main
git push -u origin main
```

> 本机未装 git 时，也可在 GitHub 网页新建仓库后用网页上传或 GitHub Desktop 提交文件夹。

---

<div align="center">

📄 许可证：[MIT](LICENSE) · 仅供个人申请使用，AI 输出需自行核对官网与事实

</div>
