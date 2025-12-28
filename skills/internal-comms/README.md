# Internal Comms Skill

這個 skill 為公司內部溝通撰寫的 AI 範本集合，可供 Claude Code CLI 自動化撰寫 3P 更新、公司通訊、FAQ 等格式文本。

## 檔案說明
- `SKILL.md`：主技能描述檔
- `.claude-skill/skill.json`：提供 metadata 給 CLI 偵測
- `examples/`：各類型格式範本
    - `3p-updates.md`：3P 更新範本
    - `company-newsletter.md`：公司通訊
    - `faq-answers.md`：常見問題回覆
    - `general-comms.md`：汎用溝通文件

## 用法
1. 在 CLI 端透過 `/internal-comms "請幫我寫..."` 指令啟動
2. 依據需求自動選擇對應範本產製內容
3. 可隨組織需求擴充範本檔

---
詳細請見上層 repo Main README。

