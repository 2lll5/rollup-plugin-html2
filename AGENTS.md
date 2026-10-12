# Agent Instructions

## Google Drive Build 交付規範（所有 Agent 必須遵守）
- **唯一目的地為 Google Drive `AI Project/rollup-plugin-html2/`**，資料夾名稱完全等於此 GitHub Repo 名稱（AI Project folder ID `1Yhfro6Ss5TSCXCVIZIHEu5h7V1gL8b27`）。`AI Project/` 頂層只應看到專案資料夾，不散放最新或舊版 ZIP。
- **專案根目錄直接放最新完整、實際建置且驗證成功的 Build**（ZIP／EXE、對應 SHA-256、全部分卷、必要安裝／還原腳本及說明）；多平台當前檔可並存。必須在新版本上傳完整並核對 Drive parent、名稱、大小、checksum 後才取代舊版；只有 checksum、少 ZIP 或少分卷的版本不完整。
- **只有重要版本差異**（重大功能、架構、美術或平台相容性）才另建 `vX.Y.Z-說明/` 子資料夾；一般舊版歸入 `歷史封存/`，不刪除。不要每次 Build 都新建版本資料夾。
- 每次開發提交 GitHub；昂貴 Actions Build 只在 `workflow_dispatch` 或正式 `release: published` 需要時觸發，避免每次 push main 都跑。交付回報版本、資料夾連結、檔案、checksum 與測試結果。
**Codex (English):** Latest complete verified build(s) directly in `AI Project/rollup-plugin-html2/`; reserve version folders for material milestones and archive routine old builds without deletion; never promote incomplete uploads.
