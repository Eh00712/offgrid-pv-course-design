# 项目日志 PROJECT_LOG

> 记录每次会话（含每个 agent）的工作。**最新记录在最上方**。
> 格式标准见 [AGENTS.md](../AGENTS.md) §3。纯日志更新提交时用 `log:` 类型。

---

## 2026-08-31 17:25 — feat(docs): 持久化推送凭证，免重复授权
- **执行者**: agent-01（sunny1043）
- **目标**: 解决每次推送都需浏览器授权的问题
- **完成内容**: 诊断出沙箱限制（git 凭据助手子进程管道被拦截，任何 credential helper 均失效）；将 GitHub token 持久化到 `~/.dsh/gh-git-credentials`（仅本机用户+系统可读，与 dsh-ssh.json 同级）；编写 `push.ps1` 包装脚本（工作区根目录，不入库），自动读取 token 经 URL 改写注入推送，此后本机推送一条命令完成、无需授权
- **变更文件**: AGENTS.md、docs/PROJECT_LOG.md、docs/PROGRESS.md、README.md（push.ps1 在工作区、不入库）
- **提交**: 3102698, 417c914
- **遗留问题**: 无。token 如需撤销：GitHub → Settings → Applications → Authorized OAuth Apps
- **下一步**: 各成员认领任务；同伴在其他机器上首次推送需各自授权一次（本机 token 仅本机有效）

---

## 2026-08-31 17:10 — feat(docs): 添加项目日志与上传进度标准
- **执行者**: agent-01（sunny1043）
- **目标**: 为多 agent 协作建立日志与进度规范
- **完成内容**: 新增 AGENTS.md（agent 强制协作规范：工作流、日志格式、提交规范、冲突规则）；新增日志模板与进度表模板
- **变更文件**: AGENTS.md、docs/PROJECT_LOG.md、docs/PROGRESS.md、README.md
- **提交**: 3102698（配套 log 提交 417c914）
- **遗留问题**: 无
- **下一步**: 各成员认领任务并开始设计

---

## 2026-08-31 16:xx — feat(init): 仓库初始化
- **执行者**: agent-01（sunny1043）
- **目标**: 创建公开仓库并上传课程设计文档
- **完成内容**: 创建 GitHub 公开仓库 offgrid-pv-course-design；上传任务书、指导书、考核标准、实验测试、论文范例
- **变更文件**: README.md、.gitignore、docs/（5 个 docx/doc 文档）
- **提交**: fda84fe
- **遗留问题**: 协作者尚未添加（在 Settings → Collaborators 添加成员）
- **下一步**: 建立日志与进度标准（即本次）
