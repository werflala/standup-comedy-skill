# standup-comedy-skill · 单口喜剧创作教练

把两本单口喜剧教材的方法论蒸馏成一个 **Agent Skill**，让你的 AI 助手（WorkBuddy / Claude Code 等）陪你从真实经历写出可上台的段子——或者诊断你的稿子为什么不好笑。

> 「没有任何一个段子是靠『重复讲』变好笑的，都是靠『改』变好笑的。」

## 它能做什么

| 你说 | 它做 |
|---|---|
| 「帮我从『健身』写个段子」 | 先问你的真实经历，按 素材→观点→前提→加梗 走完创作链，交付标注好结构的稿子 |
| 「这个段子为什么不好笑」 | 按复盘八问逐条诊断，给「问题→原理→改后版本」 |
| 「陪我想观点」 | 当段子伙伴：why / how / what else 连环追问，不替你下结论 |
| 「周五要上台 5 分钟」 | 好差好差排序法 + 计时 + 过渡取舍 |
| 「昨晚开放麦冷场了」 | 冷场五因定位 + 复盘 + 删减建议 |
| 「想办开放麦」 | 场地/布置/票务/流程全套参数 |

**设计原则**：它是教练不是代笔——段子的好笑来自你自己的观点和经历，它只负责给方法、卡标准、追问、改稿，不替你编经历。

## 方法论骨架（30 秒版）

- **四要素**：好笑 · 真实 · 原创 · 对话
- **段子公式**：段子 = 铺垫（预期）+ 包袱（违背预期）；笑 = 紧张的释放
- **观点公式**：观点 = 事实 + 负面情绪（「难怪怕蠢」四角度）
- **前提规则**：铺垫 = 主题 + 态度 + 前提；前提里不出现「我」；每天 10 条
- **加梗六法**：呈现 / 比喻 / 类比 / 夸张 / 假设 / 混合
- **红线**：不摞叶子、不套梗、公共观点要有新角度

完整细则见 [`references/`](references/)。

## 安装

### WorkBuddy

```bash
# Windows / macOS 通用：复制到用户技能目录
git clone https://github.com/werflala/standup-comedy-skill.git
mkdir -p ~/.workbuddy/skills && cp -r standup-comedy-skill ~/.workbuddy/skills/standup
```

重启会话后说「/standup」或「帮我写个段子」即可触发。

### Claude Code

```bash
git clone https://github.com/werflala/standup-comedy-skill.git
cp -r standup-comedy-skill ~/.claude/skills/standup
```

## 目录结构

```
standup/
├── SKILL.md                      # 入口：模式路由 + 核心方法卡 + 输出格式
└── references/
    ├── creation.md               # 素材五原则 / 观点提炼 / 难怪怕蠢 / 前提 / 追问法
    ├── joke-mechanics.md         # 预期违背 / 加梗六法 / CallBack / 原创红线
    └── performance.md            # 打磨三步 / 排序 / 冷场五因 / 复盘八问 / 运营参数
```

## 来源与致谢

方法论蒸馏自两本公开出版的单口喜剧教材（2018-2019）：

- 教主《人人都能学会单口喜剧》（单立人喜剧，故事体教材）
- 石老板《单口喜剧表演手册》V1.1（教材体手册，方法论上游为 Judy Carter《喜剧圣经》）

本仓库**只包含方法论的提炼、重组与个人笔记式表达，不含原书文本**；引用的个别短句（如「能表演的不叙述」）均为原书标注语录，仅作方法论说明。请支持正版。

## License

[MIT](LICENSE)
