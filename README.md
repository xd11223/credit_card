# 信用卡渠道與代理結算系統

這個資料夾是本專案的共同工作區，也是跨裝置、跨對話使用的專案記憶。

## 從這裡開始

1. 先閱讀 [docs/START_HERE.md](docs/START_HERE.md)。
2. 查看 [docs/CURRENT_STATUS.md](docs/CURRENT_STATUS.md) 了解目前進度與下一步。
3. 新需求寫入 `docs/REQUIREMENTS.md`；正式定案才寫入 `docs/DECISIONS.md`。
4. 尚未確認的內容放在 `docs/OPEN_QUESTIONS.md`，不要先當成定案實作。

## 資料夾結構

```text
.
├── AGENTS.md                  # AI/Codex 在本專案的工作規則
├── README.md                 # 人員入口
├── docs/
│   ├── START_HERE.md         # 新裝置、新對話的最短入口
│   ├── PROJECT_CONTEXT.md    # 專案背景與系統邊界
│   ├── REQUIREMENTS.md       # 已知功能需求
│   ├── DECISIONS.md          # 已確認決策與理由
│   ├── OPEN_QUESTIONS.md     # 尚待業務確認事項
│   ├── CURRENT_STATUS.md     # 現況、最近異動、下一步
│   ├── GLOSSARY.md           # 名詞定義
│   ├── SYNC_GUIDE.md         # 跨裝置同步方式
│   └── meeting-notes/        # 會議或聊天整理
└── .gitignore                # 避免金鑰與敏感資料進版控
```

## 重要安全原則

- 不要把 API 密鑰、密碼、私鑰、完整卡號、CVV 或真實付款資料提交到此資料夾。
- 測試資料應使用假資料或上游提供的測試卡號。
- 原始聊天附件如含個資，先去識別化再放入專案。

