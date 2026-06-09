# vpr-agent-radar

VPR 论文每日雷达。每天由一个远程 Claude Code 定时 agent 联网检索四个方向的**新**论文,有新货才写日报、commit & push;push 触发 GitHub Actions 自动把日报邮件发到 `ziningl@mit.edu`。

## 检索方向
1. **VPR**(Visual Place Recognition,视觉位置识别)新论文
2. **Agent 做检索**(agentic / LLM-agent retrieval)
3. **Agent 做图像检索**(agentic image retrieval)
4. **Agent 做细粒度检索**(agentic fine-grained retrieval)

## 目录
- `digests/YYYY-MM-DD.md` —— 每日日报(只在当天有新论文时生成)
- `seen.md` —— 已收录论文清单(arXiv id / 标题),用于跨天去重,避免重复推送
- `.github/workflows/email-digest.yml` —— push 到 `digests/` 时把当天日报邮件发出

## 邮件配置(GitHub Actions Secrets)
- `MAIL_USERNAME` —— 发信 Gmail 地址
- `MAIL_PASSWORD` —— 该 Gmail 的应用专用密码(App Password)
- 收件人 `ziningl@mit.edu` 写死在工作流里

## 运行机制
定时由 Claude Code「远程 routine」驱动(每天 01:00 UTC = 北京时间 09:00)。
管理入口:https://claude.ai/code/routines
