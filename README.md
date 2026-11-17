# biz-master-apply · 商科硕士 DIY 申请 Skill

一个可导入 AI Agent（Claude Code / Kimi Code 等支持 Agent Skills 的工具）的技能包，把商科硕士申请的完整流程固化为可复用指令：选校定位、PS/SOP 文书、CV、推荐信、面试模拟、套磁邮件、时间线与材料核对。不用每次复制大段 Prompt，激活后直接对话即可。

## 适用对象

准备申请金融 / 会计 / 商业分析 BA / 管理 / 经济等商科硕士的 DIY、半 DIY 申请者（27fall 及以后通用）。

## 目录结构

```
biz-master-apply/
├── SKILL.md                     # 核心：元数据 + 工作原则 + 分阶段流程
├── README.md                    # 本说明
├── LICENSE                      # MIT 许可证
├── .gitignore
├── assets/                      # 模板与可直接使用的 Prompt
│   ├── profile-template.md      # 个人背景填写模板
│   ├── prompts.md               # 各环节 Prompt 模板（选校/文书/CV/推荐信/面试/进度）
│   ├── ps-outline.md             # PS/SOP 五段大纲模板
│   ├── cv-template.md            # 申请 CV 结构模板
│   └── letter-rec.md            # 推荐信框架模板
└── references/                  # 按需加载的详细参考
    ├── school-selection.md      # 选校评估维度与方法
    └── interview-questions.md  # 商科面试题库与回答框架
```

## 安装方式

### 方式一：克隆仓库后放入 Skill 目录
```bash
git clone <你的仓库地址>
```
把整个 `biz-master-apply` 文件夹复制到对应工具的 skills 目录：

| 工具 | Skill 目录位置 |
|---|---|
| Claude Code | 项目或用户目录下 `.claude/skills/` |
| Kimi Code | 按其 CLI 文档的 skills 目录 |
| 其他兼容 Agent Skills 的工具 | 参考各自文档的 skills 加载路径 |

### 方式二：下载 ZIP 解压
在 GitHub 页面点 `Code → Download ZIP`，解压后把 `biz-master-apply` 文件夹放进上述 skills 目录。

### 方式三：直接读取（不装目录也能用）
把 `SKILL.md` 内容作为系统/角色指令贴进对话，再按需引用 `assets/`、`references/` 里的文件。

## 使用方法

1. 首次激活后，先按 `assets/profile-template.md` 填好个人背景发给 AI。
2. 直接说目标环节即可，例如：
   - "帮我做选校定位，出冲稳保清单"
   - "基于我的素材出 PS 大纲"
   - "把这段实习改成 CV 英文要点"
   - "扮演严格面试官，开始模拟面试"
   - "帮我倒排申请时间线"
3. 各环节现成 Prompt 见 `assets/prompts.md`。

## 工作原则（已写入 SKILL.md）

- AI 只做信息整理、搭框架、润色语言；**不编造**成绩、经历、数字、教授、课程、录取案例。
- 不做保录承诺；推测性结论标注"需核实"。
- 文书走三步：用户脑暴素材 → AI 出大纲 → 用户自写、AI 锁语气润色。
- 截止日期、先修课、学费、语言要求等**以院校官网当年信息为准**。
- 推荐信必须推荐人知情并确认，不虚构互动。

## 上传到 GitHub（本地初始化）

```bash
cd biz-master-apply
git init
git add .
git commit -m "feat: 商科硕士 DIY 申请全流程 Skill"
# 在 GitHub 新建仓库后，按提示关联并推送：
git remote add origin <你的仓库地址>
git branch -M main
git push -u origin main
```

> 若本机未安装 git，可先在 GitHub 网页新建仓库，再用网页上传或 GitHub Desktop 提交本文件夹。

## 自定义建议

- 把你的固定背景直接写进 `SKILL.md` 第 1 节，省去每次填写。
- 按目标地区/方向在 `references/` 里补充专属案例与项目清单。
- 新增环节时，把长模板放到 `assets/` 或 `references/`，主 `SKILL.md` 保持精简（建议 500 行以内）。

## 许可证

MIT，详见 [LICENSE](LICENSE)。
