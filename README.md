# Claude Code Skill Collection

這個專案是 Claude Code CLI 的技能資源集合（skill collection），面向團隊/企業內的自動化溝通、範本、內部文件輔助。

## 結構

```
claude-code-skill/
├── skills/
│   └── internal-comms/
│       ├── SKILL.md      # 技能描述檔
│       ├── .claude-skill/
│       │   └── skill.json # 技能 metadata，給 CLI 掃描與註冊用
│       └── examples/
│           ├── general-comms.md
│           ├── 3p-updates.md
│           ├── company-newsletter.md
│           └── faq-answers.md
├── LICENSE
└── README.md
```

## 如何在 Claude Code CLI 上同步

1. `git clone https://github.com/yourusername/claude-code-skill.git`
2. 在 Claude Code CLI 設定技能 marketplace 檔案或 config，掛載本 repo 中的 `skills/` 目錄
3. CLI 會自動掃描 `skills/*/.claude-skill/skill.json` 資訊，自動載入技能
4. 直接執行（例如）：

```bash
claude /internal-comms "請幫我寫一份3P更新"
```

## 重要說明
- 每個 skill 子目錄都必須有 .claude-skill/skill.json metadata。
- SKILL.md 為核心描述，examples/ 為指令範本或格式模板。

## 開發/貢獻方式

1. Fork 本專案
2. 每新增一個技能請建一層 `skills/your-skill/` 目錄
3. 撰寫對應的 SKILL.md 及 .claude-skill/skill.json
4. 新增範本或範例至 examples/
5. PR 回主倉庫！

## 授權
MIT License（詳見 LICENSE）
