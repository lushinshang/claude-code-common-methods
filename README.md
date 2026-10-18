# Claude Code 常用方法：遇到什麼情況，該用哪一招

依實際工作順序整理的六個情境：開工、動手前、做的時候、走歪了、對話變長、常做的事想交出去。每個情境說明什麼時候用、指令怎麼打、哪裡容易踩坑。事實與指令以 Anthropic 官方文件為準並附連結；EP431 影片只用來決定取材順序。

網頁版：https://lushinshang.github.io/claude-code-common-methods/（2026-10-18 發布；本機保留 research／qa 製作紀錄，不上傳）

## 200字介紹

想把 Claude Code 用順，常常卡在功能很多，卻不知道這個時候該用哪一個。這篇導讀依實際工作順序整理成六個情境：開工、動手前、做的時候、走歪了、對話變長、常做的事想交出去。每個情境說明什麼時候用、指令怎麼打、哪裡容易踩坑，章末附一件今天就能做的事。事實與指令以 Anthropic 官方文件為準並附連結，指令與旗標另外用腳本對過官方文件；EP431 影片只用來決定取材順序。最後一節是作者自己的使用紀錄，對照本文的建議，列出哪幾處做法不同、看完之後改了什麼、哪些還沒做到。

## 檔案說明

| 檔案 | 說明 |
|------|------|
| `claude-code-common-methods.md` | 導讀正文（Markdown） |
| `index.html` | 單檔網頁版，瀏覽器直接開啟即可閱讀（不依賴外部函式庫） |
| `images/web/` | 導讀配圖（WebP）：hero 僅 16:9（圖內無字）；fig0–fig6 各有 16:9 與 9:16 兩版，手機自動切換 |
| `images/og.png` | 分享預覽圖（由 hero 置中裁切，1200×630） |
| `share_post.md` | 社群（LINE）分享文 |
| `README.md` | 本檔 |

`research/` 與 `qa/` 只留本機，不發布。

## 原始素材

- 影片：EP431 - Claude Code 18 個用法：小白第一天就該會的，跟贏過 80% 人的進階技巧（AI 懶人報），https://www.youtube.com/watch?v=n2IIcjGC8MQ

## 查證來源

以下官方文件皆於 2026-10-18 讀取；版本門檻以文件當日內容為準。

- [Best practices for Claude Code](https://code.claude.com/docs/en/best-practices)
- [Choose a permission mode](https://code.claude.com/docs/en/permission-modes)
- [Checkpointing](https://code.claude.com/docs/en/checkpointing)
- [Model configuration](https://code.claude.com/docs/en/model-config)
- [Manage costs effectively](https://code.claude.com/docs/en/costs)
- [Store instructions and memories](https://code.claude.com/docs/en/memory)
- [Context window](https://code.claude.com/docs/en/context-window)
- [Keep Claude working toward a goal](https://code.claude.com/docs/en/goal)
- [Interactive mode](https://code.claude.com/docs/en/interactive-mode)
- [Extend Claude with skills](https://code.claude.com/docs/en/skills)
- [Hooks reference](https://code.claude.com/docs/en/hooks) 與 [Hooks guide](https://code.claude.com/docs/en/hooks-guide)
- [Subagents](https://code.claude.com/docs/en/sub-agents)
- [Review locally with /code-review](https://code.claude.com/docs/en/code-review-local)
- [Commands](https://code.claude.com/docs/en/commands)
- [Worktrees](https://code.claude.com/docs/en/worktrees)
- [Run Claude Code programmatically](https://code.claude.com/docs/en/headless)
- [CLI reference](https://code.claude.com/docs/en/cli-reference)
- [Sessions](https://code.claude.com/docs/en/sessions)

「我的做法」一節是作者自己的使用紀錄（本機最近 50 個 session 的統計），沒有公開的原始資料可供查證。
