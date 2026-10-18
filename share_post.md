想把 Claude Code 用順，常常卡在一件事：功能很多，卻不知道這個時候該用哪一個。

我對照 Anthropic 官方文件，依工作順序整理成六個情境：

・開工：CLAUDE.md 只留它猜不到的
・動手前：plan mode，大功能先讓它訪談你寫 SPEC.md
・做的時候：給它能跑的檢查，讓它自己驗收
・走歪了：Esc、/rewind，糾正兩次還錯就 /clear
・對話變長：/compact、/btw 和 subagent 管好 context
・常做的事：寫成 skill、hook，或用 claude -p 批次跑

每個情境都有可複製的指令和常見踩坑，指令與旗標都用腳本對過官方文件。最後一節是我自己多做的幾招：驗收指令先拿壞輸入試過、/goal 條件用模板寫、Stop hook 驗證關卡，連同我踩到的坑一起分享。

完整導讀：https://lushinshang.github.io/claude-code-common-methods/
