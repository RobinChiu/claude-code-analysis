# Claude Code 分析

本儲存庫包含 Claude Code（Anthropic 官方的 Claude CLI 工具）的配置和系統檔案。它為 Claude 通過 CLI 界面與使用者互動時的理解和能力提供了基礎。

## 儲存庫結構

### [system_prompt/](system_prompt/)

包含定義 Claude Code 行為和能力的系統提示：

- **system_prompt_1.md**：主要系統提示，定義核心功能、安全指南、回應風格等
- **system_prompt_2.md**：專門用於 git 歷史分析的提示
- **system_prompt_3.md**：用於對話主題檢測的提示
- **system_prompt_4.md**：用於簡潔對話摘要的提示

[更多詳情](system_prompt/README.md)

### [user_messages/](user_messages/)

包含自動插入到使用者訊息中的系統提醒模板：

- **before.md**：插入到使用者訊息開頭的提醒
- **after.md**：插入到使用者訊息結尾的提醒

[更多詳情](user_messages/README.md)

### [tools/](tools/)
![image](https://github.com/RobinChiu/claude-code-analysis/blob/main/image/tools.png)

包含 AI 助手的工具定義：

- **tools.csv**：定義了 14 種可用於 AI 助手的工具，包括它們的描述和參數規格

[更多詳情](tools/README.md)

## 目的

本儲存庫作為 Claude Code 的配置骨幹，定義了：

1. **系統行為**：Claude 應如何回應、使用什麼語調以及採取什麼行動
2. **使用者互動**：如何處理使用者訊息並添加系統提醒
3. **可用工具**：Claude 可以使用哪些工具來協助軟體工程任務

這些組件共同使 Claude Code 能夠作為一個有效的軟體工程任務 CLI 工具運作，提供符合 Anthropic 指南和使用者期望的一致行為。
